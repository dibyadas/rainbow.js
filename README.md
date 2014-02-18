Rainbow.js ![](http://img.shields.io/badge/Version-0.0.3-brightgreen.svg)
==========

A jQuery library to manage gadients easily ! 

#Get started
Its easy, you have to download the rainbow.js main script, once its done, you just have to link it to your documents, after the jQuery inclusion.

`<script type="text/javascript" src="path/to/rainbow.js"></script>`

#Create your first gradient !

Let's start with a simple structure. We will create a regular shape, a square.`

First, the css

`.square{ width:4em; height:4em; margin:.5em; }`

And the HTML : 
`<div class="square rainbow" id="gradient_2" data-type="linear" data-degrees="45" data-color="f1c40f-d35400" data-opacity="1" ></div>`

#Result : 

![](http://puu.sh/6ZyjF.png)

#Gradient Headers : 
You can add some sexy gradients to your header images. 
For example, the header image of the rainbow.js demo website use this function, so if we look at the code, we can see : 

HTML : 
````
<div class="rainbow" id="rainHeader_1" data-type="linear" data-degrees="45" data-color="f1c40f-e74c3c" data-opacity=".75" role="header"> 
	<div class="content header">
		<h1>Rainbow.js</h1>
        <h2>A small jQuery gradient helper.</h2>
    </div>
</div>
````
The image was declared on the stylesheet : 

CSS: 
````
//I use the role attribute. But assume it works with any kind of targetting. ID / Classes / attributes.
[role="header"] {
    background: url(path/to/my/image.jpg) no-repeat center center;
    background-size: cover;
    height: 15em;
    text-align: center;
}
````
#Result :
![](http://puu.sh/70Znx.png)


#Gradient images : 

This is one of the coolest Rainbow.js feature ! Its still in developement because we encounter issues with the gradient images on resize, but be sure it'll be fixed soon on a future release. 

By the way, you can still use it and play with it, but we didn't recommend to use it for production websites. 

CSS :
`.image{ width:15em; height:8em; display:block; margin:auto; background:url(image.png)no-repeat center center; background-size:cover; }`
HTML : 
`<div class="image rainbow" id="gradient_80" data-type="linear" data-degrees="45" data-color="000-F00" ></div>`
Result : 
![](http://puu.sh/6ZyEw.png)

#Gradient texts :  ![](http://img.shields.io/badge/--Webkit---ONLY-red.svg)
And finally, the last feature, a cool one, but unfortunately **-webkit-only**. 
If you're not a webkit browser user, you will get a gradient background behind your texts. 

We don't know yet if we should remove the function if you're not on a webkit browser, or display something else instad. 

HTML : 
`<h1 class="rainbow" id="rainText_1" data-type="linear" data-degrees="0" data-color="000-F00" >Look ma ! A Rainbow text !</h1>`

Result : 
![](http://puu.sh/6ZyMM.png)

