# interactive touchscreen kiosk

This repository offers touchscreen user-interface templates for interactive kiosk displays. Please fork repository and comment/push useful changes upstream.  

## **Hardware/Software Requirements**

### ACER T272HL LCD Touchscreen Monitor

* 1920x1080
* HDMI Cable
* USB Keyboard Cable

### Chromebook 
Lenovo Touchscreen Duet or 110e (potential local storage will depend on file size.)
[Pitt Wireless Chromebook Configuration](https://www.technology.pitt.edu/help-desk/how-to-documents/pittnetwireless-configuring-acer-and-samsung-chromebooks) 

### Kiosk Chrome App

[Kiosk Chrome App](https://chrome.google.com/webstore/detail/kiosk/afhcomalholahplbjhnmahkoekoijban)


[Instructional Video](https://youtu.be/M5US4OcVnL4) 

(Remember. Hold ctrl+a to access admin password.)

## System Considerations

GitHub won't host videos and you probably don't want to host them on YouTube. You can host them on your Pitt Linux server. Additionally, you could run the kiosk through the local files on your chromebook. 

-For our project presentations, you'll run your project on either a Lenovo Duet Touchscreen Chromebook or a Lenovo 110e attached to our dedicated ACER T272HL display. 


 ## Useful Code Snippets
 
 Sorry. At the moment, image carousel requires either auto-play or user controls. See [W3 carousel tutorial](https://www.w3schools.com/howto/howto_js_slideshow.asp).  
 
 Time-out function

```
<!--Place within <HEAD></HEAD>. Refreshes index.html after 180 seconds-->
  <meta http-equiv="refresh" content="180;url=index.html"> 
```
 
 Stop video from playing in modal window. 
 
 </script>

```
 <!-- Stops video/audio from playing on modal close -->
  <script>
  $(function(){
  $("body").on('hidden.bs.modal', function (e) {
  var $iframes = $(e.target).find("iframe");
  $iframes.each(function(index, iframe){
  $(iframe).attr("src", $(iframe).attr("src"));
  });
  });
  });
  </script>
```
 




