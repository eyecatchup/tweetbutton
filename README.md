tweetbutton
===========

A custom tweetbutton with tweet count.

This implementation consist of 3 parts:
 * HTML Markup 
 * CSS Styles  
 * JavaScript (jQuery)  

== Background  

The official Twitter JavaScript Tweetbutton-Widget has a bug. When you implement the official Twitter Tweet-Button and also the Facebook Like-Button, the Google+ +1-Button or any other iframe object within the same page, you will notice that the Tweet-Button JavaScript code is attempting to traverse every dom object on the page and it is not able to access the other iframe object(s). Thus, you will see an `Unsafe JavaScript attempt to access frame with URL %domain from frame with URL http://example.com/. Domains, protocols and ports must match.` error message in your JS console.  

Though it doesn't impact the functionality, if you do not want to just ignore it, this project provides an alternative. The code renders a Tweet-Button with the exact same style of the official Tweet-Button and, unlike other custom implementations, also includes the tweet count for the current URL. 
 
== Demo

http://fiddle.jshell.net/eyecatchup/Th6P2/2/show/ 
 
Copyright: 2013 - present, Stephan Schmitz <eyecatchup@gmail.com>  
License:   http://eyecatchup.mit-license.org/  
