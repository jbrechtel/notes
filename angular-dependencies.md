### Angular is magic

Not sure how but Angular.js figures out dependencies by function argument names. You don't really rely on this in the real world because minification obviously breaks this, but the interesting bit is that I didn't know Javascript exposed this information. Via reflection? Or is Angular reading the javascript directly? That'd be stupid.

