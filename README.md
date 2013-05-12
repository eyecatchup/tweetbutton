# A custom tweetbutton (with tweet count)

This implementation consist of 3 parts:
 * HTML Markup 
 * CSS Styles  
 * JavaScript (jQuery) 

## Demo

http://fiddle.jshell.net/eyecatchup/Th6P2/2/show/

## Background  

The official Twitter JavaScript Tweetbutton-Widget has a bug. When you implement the official Twitter Tweet-Button and also the Facebook Like-Button, the Google+ +1-Button or any other iframe object within the same page, you will notice that the Tweet-Button JavaScript code is attempting to traverse every dom object on the page and it is not able to access the other iframe object(s). Thus, you will see an `Unsafe JavaScript attempt to access frame with URL %s from frame with URL %s. Domains, protocols and ports must match.` error message in your JS console.  

Though it doesn't impact the functionality, if you do not want to just ignore it, this project provides an alternative. The code renders a Tweet-Button with the exact same style of the official Tweet-Button and, unlike other custom implementations, also includes the tweet count for the current URL. 

**Update (12.05.2013)**: In <a href="https://dev.twitter.com/discussions/17168" target="_blank">a recent discussion</a> on dev.twitter.com, <a href="https://dev.twitter.com/discussions/17168#comment-38577" target="_blank">a Twitter Dev commented</a> on that *"issue"*:  


> So, the security warning is an ugly but unfortunately inevitable consequence of the messaging system used to power the current version of Web Intent Events. [..]
>  
> However, it's not an error, in so far as it's not actually breaking functionality [..].
>  
> As someone who spends a substantial amount of his day staring at the JavaScript console, rest assured I find it annoying as well, but it's an unfortunate case that WebKit has started being more aggressive about the warnings without providing a cleaner API for finding the right frame to send messages to.
>  
> That said. We are going to reimplement the messaging system in the near-ish future (see last months IE6 and IE7 deprecation notice) and the current design I'm working on will not trigger these annoying messages. So my hope is that although it's not really a error now, it'll still be tidier in the future.

When the reimplementation goes live, I will put a note and link on this page. Until then, feel free to use my implementation.

## Legal
 
Copyright: 2013 - present, Stephan Schmitz <eyecatchup@gmail.com>  
License:   http://eyecatchup.mit-license.org/  
