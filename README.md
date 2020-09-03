# NPT
Native PHP Templating

************************************************************************************************************************

this can probably be phrased better but im just gonna spill the beans for now.<br>
templating engines like smarty, twig, blade, (...etc), are (imo) a bad way to do templating.<br><br>
problem 1: if you don't use caching chances are its gonna be very slow to serve a page.<br>
problem 2: seperation of concerns is the main reason to use a template engine <br>
but in the end it is not enough, you still have to put logic in the template.<br>
problem 3:  learning a new syntax is annoying, especially for non-developers, like designers, <br>
who will probably have to deal with a template engine in their HTML.<br><br>
solution: use a dedicated library to get the template .html files you need, parse the .html files with what variables <br>
you need in the php script and respond with the parsed html.<br><br>
PHP has DOM manupulation tools, and this is why its native, its all there already, but the tools are too verbose compared to todays template engine. this library will use the PHP DOM extension to give performant templating tools that are easy to work with. this might be a bad idea or even not work at all, and it might be the way everyone will work in the future.<br><br>
the following article is the reason i decided to try this and it does a much better job at explaining this idea.<br>
https://benkoworks.com/your-templating-engine-sucks-and-everything-you-have-ever-written-is-spaghetti-code-yes-you/<br>
even though this article is almost a decade old by now, i think its still relevant today.
