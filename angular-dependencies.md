### Angular is magic

> Not sure hwo but Angular.js figures out dependencies by function argument names.
> This means that Javascript exposes parameter names via reflection? Either that or Angular
> is reading the JS source? Either way, this doesn't work when using minification.
> So, instead, make your controllers a function object and give them an $inject property. Specify
> their dependencies that way.
