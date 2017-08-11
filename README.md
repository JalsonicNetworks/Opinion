Jalsonic Server Maintenance Notice! - All Jalsonic servers will be undergoing Scheduled Maintenance for about 3 days. During these hours servers are temporarily unable. We apologize for the inconvenience.
------------------------------

![Jalsonic Opinion](http://jalsonic.com/assets/github/githugOpinionHeader.png)

Jalsonic Opinion Version v1 Beta - Build something amazing
===================

Jalsonic Opinion does not have any dependencies on a JavaScript framework. Jalsonic opinion is completely free to download and also works in IE 9+, Edge 11+, Firefox 2+, Safari 3.2+, Chrome 3+, and Opera 12+. 

What Does Opinion Do, Exactly?
------------------------------

Good question! I'm so glad you asked.

Opinion (o-) is a modern and powerful front-end framework with built-in responsiveness.It Uses standard CSS for Speeds up mobile HTML apps, Removes the inconsistent styling of HTML elements provided by browsers and Provides equality CSS for all devices. PC, laptop, tablet, and mobile. A secure way for developers to enjoy the benefit of a responsiveness, network and geolocation objects and animation websites and mobile web application.

If you want to find out the IP address, Operating system , Browser of an Internet user using the devise through JavaScript, you can use  opinion objects or to get an idea what part of the country or world because sometimes you can give specific instruction to internet user.

On-scroll animations are one of the most popular and enduring web-development techniques from recent years. Jalsonic Opinion helps you to create on-scroll animation website and mobile web application, you can use opinion moves because animation that makes your site look dynamic and modern, unlike the static pages of old.

Works Everywhere
----------------------

Opinion is a cross-browser front-end framework for the websites and mobile web application, that's easy to use and easy to deploy. It works on all major Internet browsers.

![Jalsonic Opinion](http://jalsonic.com/assets/github/crossbrowser.jpg)


Opinion Initialization
----------------------

A few things you should do to start creating awesome websites and mobile web application with powerful front-end opinion framework. First load the opinion JavaScript file if you haven't already loaded it. Opinion does not have any dependencies on a JavaScript framework. 
 
Add the following link to your page code. Copy and paste this script tag on your html document file.

  ```html
    <script src=" //opinion.jalsonic.com/svn/base/version/01/opinionsource"></script>
  ```
This is an ultra-small bit of JavaScript that enables you to load opinion Classes and attribute on HTML tag of your page.

**There are two ways to enable the features of opinion.**

Before adding the link you can use the following code for application initialization in your all pages of your websites and mobile web applications:

  
  ```javascript
    <script> 
    	window.opinion = function() { 
    	   		o.init({
    				dirpath : "",  // Path of opinion files directory
    				drawing : "", // drawing mode 
    				viewport : "",  // browser rendering engine
    				googleanalytics : "", add google analytic Id to analyes your web 
    				mediaquery : ""  // enable stander media query styles sheets 
    			}); 
    	}; 
    </script>
  ```

Other way is that to make external calls for your specific page you need to use Opinion attribute on HTML Tag to enable the features of Opinion. This will help you.

  <html opinion-dirpath="" opinion-drawing="" opinion-mediaquery="" opinion-viewport="" opinion-googleanalytics=""> 

> Note: if you will using opinion attribute it will works on current page where you written.

 - **About `o.init(Object parameter)` and Opinion HTML attribute**

 - **Dirpath**

Opinion dirpath process scans all files, folders and allows automatically select opinion resources to include the process

**In HTML  tag.**

  ```html
    <html opinion-dirpath="/opinion">
  ```

**In o.init() Method**

  ```javascript
    window.opinion = function() { 
      	o.init({
		    dirpath : "/opinion",  // Path of opinion directory
		    ..
	    }); 
    }; 
  ```

 - **Drawing**

Very helpful when your site is in development and testing. Opinion makes a line on the top of the page to show exact screen dimensions of smartphones, tablets and computers. You can change the layout of your websites and mobile web applications based on these lines. This will help you:

 - Blue line is for .portrait-SmartPhone dimensions 480px
 - Red line is for .landscape-Smartphone and .portrait-Tablet dimensions 768px
 - Yellow line is for .landscape-Tablet and .desktop dimensions 992px
 - Green line is for .large-Desktop dimensions larger then 1024px

> Note: opinion generating these classes automatic when your pages is loading.

**In HTML  tag.**

  ```html
    <html opinion-drawing=" integer - 1 for enable 0 for disable ">
  ```

**In o.init() Method**

  ```javascript
    window.opinion = function() { 
    	o.init({
	    drawing: "1",  // integer - 1 for enable 0 for disable
	    ..
	}); 
    }; 
  ```

- **Viewport**

The viewport is a virtual area used by the browser rendering engine to determine how content is scaled and sized when it is initially rendered on the current screen. This will help you:

**In HTML tag**

  ```html
  <html opinion-viewport="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" /> 
  ```
	
**In o.init() Method**

  ```javascript
    window.opinion = function() { 
       	o.init({
	    viewport: " width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no ",  // rendering engine to determine 
	    ..
	    }); 
    }; 
  ```

 - **Googleanalytics**



Very easy way to implement Google analytics in your website and mobile web applications in a seconds. Get the data you need to make intelligent marketing and business decisions with Google Analytics. This will help you:

**In HTML tag**

  ```html
  <html opinion-googleanalytics="UA-xxxx-xx" /> 
  ```
	
**In o.init() Method**

  ```javascript
  window.opinion = function() { 
    	o.init({
    	googleanalytics: "UA-xxxx-xx",  // Google analytics tacking Id..
    }); 
  }; 
  ```

Object Properties  | Comments
------------- | -------------
o.googleAnalytics.id  | Your Google analytics Id 
o.googleAnalytics.status  | Return Number - 200 for Successful responses, 404 for cannot find analytics request. 

 - **Mediaquery**

Opinion has an external style sheet to define different style rules for different media types/devices for comman devices. This will help you:

    /custom.css for all devices.
    /large-desktops.css for large desktop max width 1200px. 
    /desktops.css for normal desktops max width 992px.
    /tablets.css for tablets max width 768px.
    /phones.css for phones max width 480px.

We use the following media queries in our grid system.

> Note: opinion generating these stylesheet link automatic when your pages is loading.

**In HTML tag**

  ```html
    <html opinion-dirpath="/opinion"  opinion-mediaquery=”1”>
  ```

**In o.init() Method**

  ```javascript
    window.opinion = function() { 
       	o.init({
		   dirpath : “/opinion”,  // Path of opinion directory
    mediaquery : “1”, // integer - 1 for enable 0 for disable
		  ..
	    }); 
    }; 
  ```


> Note: by defult path of mediaquery files is this opinion/css/xxx.css. If you have opinion folder in the other dirtory use dirpath to allows automatically select opinion resources to include the process.

Opinion Built-In Responsiveness
-------------------------------

The Opinion includes a responsive, grid system allows up to 12 columns to handle your layout across the page, and the columns will re-arrange automatically depending on the screen size.

The opinion grid system has four classes:

 - Extra small devices Phones we will use the `.o-col-s-1` to `.o-col-s-12`
   classes (for phones)
 - Small devices Tablets  we will use the  `.o-col-m-1` to `.o-col-m-12`
   classes (for tablets)
 - Medium devices Desktops  we will use `.o-col-l-1` to `.o-col-l-12` classes
   (for desktops)
 - Large devices Desktops  we will use `.o-col-xl-1` to `.o-col-xl-12` (for
   larger desktops)

See how aspects of the opinion grid system work across multiple devices with a handy table.

 .| Extra small devices Phones (<768px)   | Small devices Tablets (≥768px) | Medium devices Desktops (≥992px) | Large devices Desktops (≥1200px) 
------------- | ------------- | ------------- | ------------- | -------------
**Grid behavior**  | Horizontal at all times | Collapsed to start, horizontal above breakpoints | Collapsed to start, horizontal above breakpoints | Collapsed to start, horizontal above breakpoints 
`.o-container` **Container width**  | None (auto) | 750px | 970px | 1170px
**Class prefix** | `.o-col-s-` | `.o-col-m-` | `.o-col-l-` |`.o-col-xl-`
**number of columns** | 12
Column width	 | Auto	 | ~62px | ~81px | ~97px
Gutter width	| 30px (15px on each side of a column)
Offsets	| `.o-col-s-offset-*` | `.o-col-m-offset-*` | `.o-col-l-offset-*` | `.o-col-xl-offset-*`  
Column ordering	| `.o-col-s-pull-*` | `.o-col-m-pull-*` | `.o-col-l-pull-*` | `.o-col-xl-pull-*` 


opinion provides various helper classes that can be useful in certain situations in dealing with grids.

**Offsetting columns:**  You can use offset classes like `.o-col-l-offset-*` or `.o-col-m-offset-*` to leave a particular number of virtual opinion columns to the left of any column (kind of like invisible place holders).

**Reordering:**  Use classes like `.o-col-m-push-*` and `.o-col-s-pull-*` to shift a column to the right or left, respectively.

For more faster and friendly development, use these utility classes for showing and hiding content by device via media query. 

`.o-xl-hidden`, `.o-l-hidden`, `.o-m-hidden`, `.o-s-hidden`, `.o-xl-visible`, `.o-l-visible`, `.o-m-visible`, `.o-s-visible`  

utility classes for toggling content when printed. 

`.o-print-visible`, `.o-print-hidden`

utility classes for showing and hiding content by modern browser. 

`.o-firefox-hidden`, `.o-chrome-hidden`, `.o-opera-hidden`, `.o-safari-hidden`, `.o-IE-hidden`, `.o-firefox-visible`, `.o-chrome-visible`, `.o-opera-visible`, `.o-safari-visible`, `.o-IE-visible`

In JavaScript you can get your visitor's/client's browser name and implement specific instructions to internet user to how your contacts shown in modern browser and you can give better user experience.


Object Properties | Return Value
------------- | ------------- 
`o.webBrowser.browser` |	String - like : firefox, chrome
`o.webBrowser.isChrome` |	Boolean - true, false
`o.webBrowser.isFirefox` | Boolean - true, false
`o.webBrowser.isOpera` |	Boolean - true, false
`o.webBrowser.isIE` |	Boolean - true, false
`o.webBrowser.isSafari` |	Boolean - true, false


Opinion network
---------------

**Getting the correct IP address with JavaScript.**

Getting real client IP address in JavaScript. Many times we need the visitor's IP address for validation, security, spam prevention, etc. Getting the Visitor's IP address is very easy in JavaScript Now. The simplest way to get the visitor's/client's IP address is using the `o.network.ip` object or get the country of visitor's/client's base on visitor's/client's  IP Address `o.network.ip` Country object.

Object Properties | Return Value
------------- | ------------- 
`o.network.ip` | Number - Your public IP address
`o.network.ipCountry` | String - Country short names without space

Opinion regions
---------------


**Showing content by regions**

Some time we need specific contents, images, fields’ of HTML form and most important area of the website and mobile web application for some regions not for all regions of the world. In jalsonic opinion is very easy to control these things now so you can give better user experience. Use ‘o-‘ with two digit ISO classes like: .o-pk for Pakistan, .o-sa for Saudi Arabia, .o-tr for Turkey. This will help you.


Example:

    //This div tag only shown in turkey  
    <div class=”o-allRegions”> International Conference on Business, Economics, Social Science & Humanities (BESSH) -
    09-10 May 2016 – Istanbul </div>

    //This div tag only shown in turkey and Pakistan 
    <div class=”o-tr o-pk”> International Conference on Business, Economics, Social Science & Humanities (BESSH) -
    09-10 May 2016 – Istanbul - or - International Conference on Business, Economics, Social Science & Humanities (BESSH) -
    09-10 May 2016 – Lahore </div>

Opinion regions classes reference 

```css
    .o-allRegions, .o-af, .o-ax, .o-al, .o-dz, .o-as, .o-ad, .o-ao, .o-ai, .o-aq, .o-ag, .o-ar, .o-am, .o-aw, .o-au, .o-at, .o-az, .o-bs, .o-bh, .o-bd, .o-bb, .o-by, .o-be, .o-bz, .o-bj, .o-bm, .o-bt, .o-bo, .o-bq, .o-ba, .o-bw, .o-bv, .o-br, .o-io, .o-bn, .o-bg, .o-bf, .o-bi, .o-kh, .o-cm, .o-ca, .o-cv, .o-ky, .o-cf, .o-td, .o-cl, .o-cn, .o-cx, .o-cc, .o-co, .o-km, .o-cg, .o-ck, .o-cr, .o-ci, .o-hr, .o-cu, .o-cw, .o-cy, .o-cz, .o-cd, .o-dk, .o-dj, .o-dm, .o-do, .o-ec, .o-eg, .o-sv, .o-gq, .o-er, .o-ee, .o-et, .o-fk, .o-fo, .o-fj, .o-fi, .o-fr, .o-gf, .o-pf, .o-tf, .o-ga, .o-gm, .o-ge, .o-de, .o-gh, .o-gi, .o-gr, .o-gl, .o-gd, .o-gp, .o-gu, .o-gt, .o-gg, .o-gn, .o-gw, .o-gy, .o-ht, .o-hm, .o-hn, .o-hk, .o-hu, .o-is, .o-in, .o-id, .o-ir, .o-iq, .o-ie, .o-im, .o-il, .o-it, .o-jm, .o-jp, .o-je, .o-jo, .o-kz, .o-ke, .o-ki, .o-xk, .o-kw, .o-kg, .o-la, .o-lv, .o-lb, .o-ls, .o-lr, .o-ly, .o-li, .o-lt, .o-lu, .o-mo, .o-mk, .o-mg, .o-mw, .o-my, .o-mv, .o-ml, .o-mt, .o-mh, .o-mq, .o-mr, .o-mu, .o-yt, .o-mx, .o-fm, .o-md, .o-mc, .o-mn, .o-me, .o-ms, .o-ma, .o-mz, .o-mm, .o-na, .o-nr, .o-np, .o-nl, .o-nc, .o-nz, .o-ni, .o-ne, .o-ng, .o-nu, .o-nf, .o-kp, .o-mp, .o-no, .o-om, .o-pk, .o-pw, .o-ps, .o-pa, .o-pg, .o-py, .o-pe, .o-ph, .o-pn, .o-pl, .o-pt, .o-pr, .o-qa, .o-re, .o-ro, .o-ru, .o-rw, .o-bl, .o-sh, .o-kn, .o-lc, .o-mf, .o-pm, .o-vc, .o-ws, .o-sm, .o-st, .o-sa, .o-sn, .o-rs, .o-sc, .o-sl, .o-sg, .o-sx, .o-sk, .o-si, .o-sb, .o-so, .o-za, .o-gs, .o-kr, .o-ss, .o-es, .o-lk, .o-sd, .o-sr, .o-sj, .o-sz, .o-se, .o-ch, .o-sy, .o-tw, .o-tj, .o-tz, .o-th, .o-tl, .o-tg, .o-tk, .o-to, .o-tt, .o-tn, .o-tr, .o-tm, .o-tc, .o-tv, .o-ug, .o-ua, .o-ae, .o-gb, .o-us, .o-um, .o-uy, .o-uz, .o-vu, .o-va, .o-ve, .o-vn, .o-vg, .o-vi, .o-wf, .o-eh, .o-ye, .o-zm, .o-zw
```

Opinion Moves Reveal
--------------------

**Scroll animations with Moves Reveal and friend Animate.css** 

On-scroll animations are one of the most popular and enduring web-development techniques from recent years to provide an interesting and interactive experience for your internet users who visits the website and mobile application. With modern sites providing a greater deal of interactivity, it’s becoming increasingly expected that even simple websites and mobile application will offer some level of animation to engage their people who visits the website.

**Implementation of Moves Reveal in your website and mobile web applications**

You can use Animate.css .you can also use online tool for creating native CSS3 Keyframes Animation. You can easily generate your own consistent CSS3 animation using simple UI without any coding.

For more detail of key frame see this link:  [click here](http://www.w3schools.com/cssref/css3_pr_animation-keyframes.asp)

    @keyframes bounceInDown { from, 60%, 75%, 90%, to { -webkit-animation-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000); animation-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000); }
      0% { opacity: 0; -webkit-transform: translate3d(0, -3000px, 0); transform: translate3d(0, -3000px, 0); }
      60% { opacity: 1; -webkit-transform: translate3d(0, 25px, 0); transform: translate3d(0, 25px, 0); }
      75% { -webkit-transform: translate3d(0, -10px, 0); transform: translate3d(0, -10px, 0); }
      90% { -webkit-transform: translate3d(0, 5px, 0); transform: translate3d(0, 5px, 0); }
      to { -webkit-transform: none; transform: none; } }
    
    .bounceInDown { -webkit-animation-name: bounceInDown; animation-name: bounceInDown; }

 
Once you have done that you can just define "**o-moves**" as the parent class to animate whichever animation is defined, here we are using "**bounceInDown**". This will help you.

    <div class="o-moves bounceInDown"></div>

Moves HTML attribute | Comments
------------- | ------------- 
movesDelay="Integer" | Integer ‘seconds’ - Delays to your animations 
movesDuration=”Integer”	| Integer ‘seconds’ - Speed of animations


For those who want to see more examples of this in action, you can visit [Jalsonic Opinion](http://jalsonic.com/opinion) and [Imranamanat](http://Imranamanat.com) website.

Designed, Built and Maintained by [Imran Malik](http://Imranamanat.com) imran@imranamanat.com and [Jalsonic Secure Team](http://jalsonic.com/secure). A Division of [Jalsonic Networks](http://jalsonic.com).


![Jalsonic Footer](http://jalsonic.com/assets/github/githubfooters.png)



