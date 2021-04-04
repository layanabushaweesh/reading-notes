## <%= EJS %>
EJS (Embedded JavaScript templating): is a simple templating language that lets you generate HTML markup with plain JavaScript.

## How to use EJS:
install.
$ npm install ejs
add it to JS file.
let ejs = require('ejs');
use it to render data to html.
add pages/index.ejs to your repo.
app.set('view engine', 'ejs');

app.get('/', (req,res)=>{
    res.render('pages/index', {
        name: req.userName
    });
})
<h1> Hello <%= name %></h1>
let template = ejs.compile(str, options);
template(data);
// => Rendered HTML string

ejs.render(str, data, options);
// => Rendered HTML string

ejs.renderFile(filename, data, options, function(err, str){
    // str => Rendered HTML string
});
Usage
let template = ejs.compile(str, options); template(data); // => Rendered HTML string

ejs.render(str, data, options); // => Rendered HTML string

ejs.renderFile(filename, data, options, function(err, str){// str => Rendered HTML string});

## Options in EJS:
cache Compiled functions are cached, requires filename.
filename Used by cache to key caches and for includes.
context Function execution context.
compileDebug When false no debug instrumentation is compiled.
client Returns standalone compiled function.
delimiter Character to use with angle brackets for open/close
debug Output generated function body
_with Whether or not to use with() {} constructs. If false then the locals will be stored in the locals object.

## EJS Tags
<% 'Scriptlet' tag, for control-flow, no output
<%_ ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it
<%= Outputs the value into the template (HTML escaped)
<%- Outputs the unescaped value into the template
<%# Comment tag, no execution, no output
<%% Outputs a literal '<%'
%> Plain ending tag
-%> Trim-mode ('newline slurp') tag, trims following newline
_%> ‘Whitespace Slurping’ ending tag, removes all whitespace after it