# EJS PARTIALS
Partials come in handy when you want to reuse the same HTML across multiple views.

EJS partials work like EJS layouts too in creating a single fix content on a web page.

Unlike EJS Layouts, EJS partials can work without the express-ejs-layouts module. EJS partials apply in cases like creating objects like header, footer, div.

For a web page to contain the partial, it must be connected to each partial via a line of code, unlike layouts which apply everywhere.

## When to use
Partials are good to use when you have HTML element that you'll reuse across multiple views (like header, footer, navbar)

## Why use partials
using partials makes it easier to track and modify your elements making sure they're still the same across all your pages.

To make the same navigation bar and footer appear in the home and the other pages:
Under the views/partials/ directory create a file callednavbar.ejs which will contain only the HTML for the navigation bar at the top of the home and post pages, and a file called footer.ejs in that same directory.
Example of how the main directory should look like:



 **Note** : The <%- %> tags allow us to output the unescaped content onto the page (notice the -). This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’, etc…


Let’s create the homepage template in views/home.ejs and include the navbar and footer partial we just created:

    <div class="container">
        <%- include('partials/navbar') %>
        <div class="jumbotron"></div>
        <div class="row"></div>
        <%- include('partials/footer') %>
    </div>


