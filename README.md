###BASIC USAGE.
Razor Slider is super simple to set up. Just create an element, and put your content inside. If your content is of different heights, razor slider will animate smoothly to accommodate it.
give it an id or class or any valid Jquery selector.
```
        <ul id="rslide">
            <li><img src="images/1.jpg" alt="1.jpg"/></li>
            <li><img src="images/2.jpg" alt="2.jpg"/></li>
            <li><img src="images/3.jpg" alt="3.jpg"/></li>
            <li><h1>Text Slide</h1></li>
            <li><img src="images/5.jpg" alt="5.jpg"/></li>
            <li><img src="images/5.jpg" alt="5.jpg"/></li>
        </ul>
```
include jQuery, the razor.slider.js or razor.slider.min.js file and the razor.slider.css or razor.slider.min.css file in the footer of your page and header of your page respectively, of course, call the function:

```HTML 
         <!-- IN HEAD -->
        <link rel="stylesheet" href="css/razor.slider.css" />

         <!-- JUST ABOVE BODY END TAG -->
        <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>
        <script src="js/razor.slider.jquery.js"></script>
        <script>
            $(function(){
                $("#rslide").razorslider();
            });    
        </script>
```

###OPTIONS.
Razor Slider includes the following options for your content sliding needs. Just include the ones you want to change.

```javascript
$("#rslide").razorslider({
   autoplay : false, //autoplay default is false set it to true to slide auto
   controls: true,  //left and right nav set it to false to hide it
   indicators: true, // small bullets at the bottom set it to false to hide it
   speed:2000, // slide speed in milliseconds
   autoplaySpeed:3000, // auto play interval speed milliseconds
   easing:'easeOutQuad', // type of easing u would like for slides
   controlRight:'&raquo;', // right control text
   controlLeft:'&laquo;', // left control text
   onSlide:function(){
    // this event triggers immediately on slide change
   },  
   onSlidePost:function(){
     // this event triggers after slide has been changed
   }
});
```
###<a href="https://riazxrazor.github.io/">Live Preview</a>
#### other easing effects

Easing is all thanx to   <a href="http://www.robertpenner.com/easing/">Robert Penners easing equations</a> 
and <a href="http://gsgd.co.uk/sandbox/jquery/easing/">jQuery easing plugin</a>
<br>for easing effects refer to http://easings.net/


* easeInQuad
* easeOutQuad
* easeInOutQuad
* easeInCubic
* easeOutCubic
* easeInOutCubic
* easeInQuart
* easeOutQuart
* easeInOutQuart
* easeInQuint
* easeOutQuint
* easeInOutQuint
* easeInSine
* easeOutSine
* easeInOutSine
* easeInExpo
* easeOutExpo
* easeInOutExpo
* easeInCirc
* easeOutCirc
* easeInOutCirc
* easeInElastic
* easeOutElastic
* easeInOutElastic
* easeInBack
* easeOutBack
* easeInOutBack
* easeInBounce
* easeOutBounce
* easeInOutBounce


Its to some extent responsive well i'm working on it.<br>
Anybody want to work on it or improve it please jump right in.
