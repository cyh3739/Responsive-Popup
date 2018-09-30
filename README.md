

# [jQuery] - Responsive Popup
\# Responsive Popup  
\# Multiple Popup  
\# Mobile Popup  
\# Simple Popup  
\# Easy Popup  

### License - MIT license ( http://opensource.org/licenses/MIT )

![ResponsivePopup
](./ResponsivePopup.jpg)
_ _ _
### [Set up]
```
<!-- jQuery -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
```

```
<!-- Css & JavaScript -->
<script src="./rpopup.min.js"></script>
<link rel="stylesheet" href="./rpopup.css">

<script>
$(document).ready(function(){
    //Single Popup
    $.rpopup({
        imgSrc : "./imgs/img1.png",
        mobile_imgSrc : "./imgs/img2.png",
        positionTop :"70px",
        positionLeft :"50%", //(Center)
        headerText :"Responsive Popup"
    });
	
});
</script>
```
( No HTML )


_ _ _
### [Multiple Popup]   
**Parameter : Objects in Array**
```
//Parameter : Objects in Array
$.rpopup([
    {
        imgSrc : "./imgs/img1.png",  
        positionTop :"70px",
        positionLeft :"50%",
        headerText :"Responsive Popup" 
    },
    {
        imgSrc : "./imgs/img2.png",  
        positionTop :"140px",
        positionLeft :"51%",
        headerText :"Responsive Popup" 
    }
]);
```
_ _ _
### [Options]
```
$.rpopup({
		imgSrc : "",               // String (Desktop Image Url) 
		mobile_imgSrc : "",        // String (Mobile Image Url)
		htmlCode : "",             // String (Html Code)
		linkHref : "",             // String (Link Url)
		linkTarget : "_self",      // String (Default : _self)
		positionTop : "",          // String or Number (Default : 30px)
		positionLeft : "",         // String or Number (Default : 30px)
		footerBar : true,          // Boolean (Default : true)
		headerText : "",           // String (Default : none)
		footerText : "",           // String (Default : "Don\'t show this again")
		buttonText : "",           // String (Default : "CLOSE")
		responsive : true,         // Boolean (Default : true)
		responsiveMaxWidth : 720   // String or Number  (Default : 720px)
});
```

___
### [Custom Style]
```
/*=== wrap ===*/
.rPopup_wrap{ border:1px solid #dee2e6; border-radius:3px; }

/*=== headerBar ===*/
.rPopup_header{ height:33px; background:#f1f3f5; }
.rPopup_header>h3>span{ font-size:17px; color:#343a40; }

/*=== footerBar ===*/
.rPopup_footer{ background:#f1f3f5; }
.rPopup_footer label span{ font-size:16px; }
.rPopup_footer button{ border:1px solid #ced4da; background:#dee2e6; padding:5px 7px; border-radius:5px; }
```
