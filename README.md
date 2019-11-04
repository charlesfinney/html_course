# html_course by Charles Finney
the purpose of this course is to go beyond the basic "Hello World" webcourse and cover all steps in creating an interactive webpage with images and media, and examples of how to drive traffic to it.
# Prerequisities 
## GitHub repo setup
### create Github account 
### create Github repo
#### click on Settings tab
at initial setting Options scroll to "GitHUb Pages" and then under <b>Source</b> select master branch /docs folder
### create the following directory folder structure
a directory/folder for <b>assets</b> used across the whole website. and a directory/folder for page specific content 
```
/assets  
  /css
  /img
  /js
/content
  /images
  /media
```
better
Create a directory structure seperating site design from content and media.
1. in the /assets folder are all files, documentation and images used in layout and navigation througout the site, in subfolders according to their type.
1. further in the /content folder are all media, files and images that make up the content of the site, also in subfolders according to type.
  
```bash

.
├── /assets
│   ├── /css
│   │   ├── main-stylesheet.css
│   │   └── normalize.css
│   │
│   ├── /doc/ = (documentation)
│   │   ├── css.md
│   │   ├── extend.md
│   │   ├── faq.md
│   │   ├── html.md
│   │   ├── js.md
│   │   ├── misc.md
│   │   ├── TOC.md
│   │   └── usage.md
│   │
│   ├── /font
|   │   └── *.ttf
│   │
│   ├── /img
│   │   ├── *.png  
│   │   ├── *.jpg
│   │   ├── *.svg
│   │   └── .gitignore
|   │   └── /soc
|   │       └── *.svg
│   │
|   └── /js
|       ├── main.js
|       ├── plugins.js
|       └── /vendor/
|           ├── jquery.min.js
│           └── modernizr.min.js
├── /content
│   ├── /audio
|   │   └── *.aac
│   │
|   └── /images
|   │       ├── /finney
|   │       │   └── *.png 
|   │       └── /tung
|   │           └── *.png 
│   ├── /pdf
|   │   └── *.pdf
│   │
│   └── /video
│       └── *.mp4
│   
├── .editorconfig
├── .htaccess
├── 404.html
├── browserconfig.xml
├── favicon.ico
├── humans.txt
├── icon.png
├── index.html
├── README.md
└── .gitignore

```
install the folowing software to enhance the website or find suitable [alternatives](https://alternativeto.net/)
## Install a free HTML Editor
Download and install a free HTML Editor like [Brackets](http://brackets.io/) or [Atom](https://atom.io/)
## Install a free image editor 
Download and install a free HTML Editor like [Brackets](http://brackets.io/) 
## Install a free audio Editor
Download and install [Audacity®](https://www.audacityteam.org/) a free, open source (cross-platform) digital audio editor, recorder, and mixer.
Apache web server, this means adding the following lines to your .htaccess
```
# AddType TYPE/SUBTYPE EXTENSION
AddType audio/mpeg mp3
AddType audio/mp4 m4a
AddType audio/ogg ogg
AddType audio/ogg oga
AddType audio/webm webma
AddType audio/wav wav
```
Webpage HTML 
```
<audio>
   <source src="elvis.mp3" type='audio/mpeg; codecs="mp3"'>
   <source src="elvis.oga" type='audio/ogg; codecs="vorbis"'>
   <!-- add your fallback solution here -->
</audio>
```
## Download & Install [Bitvise](https://www.bitvise.com/download-area)
a secure remote access software for Windows for uploading files and direcotries from your computer to your web hostinf service
# Website Marketing and IOT integration
## QR code 
## NFC 
## Flyer/ Poster/ artwork

# Infostructure
# HTML 
```
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>pageTitle</title>
  <link rel="stylesheet" href="default.css">
  <script src="default.js"></script>
</head>
<body>


<div id="accessibility">
  <a href="#nav">Skip to Navigation</a> |
  <a href="#main-content">Skip to Content</a>
</div>


<header role="banner">
  <div class="masthead">
    <a href="#"> ....site title or logo, purposely not an h1.... </a>
  </div>
  <nav id="nav">
    <ul>
      <li><a href="#">
        ....main site nav list....
      </a></li>
    </ul>
  </nav>
  <div id="secondary-nav">
    <ul>
      <li><a href="#">
        ....other non-primary navigation doesn't belong in a nav element....
      </a></li>
    </ul>
  </div>
</header>


<section id="main-content" role="main">
  <h1> ....page title here.... </h1>
  <article>
    <header>
      <h2>....article heading if needed....</h2>
      <h3>....article sub-heading if needed....</h3>
    </header>
    ....article content here....
  </article>
  <article>
    ....use more article elements if appropriate; if not, I still use divs....
  </article>
</section>


<aside id="sidebar">
   ....site sidebar here....
</aside>


<footer>
  .... footer content here ....
</footer>


</body>
</html>
```
or 
```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
	
	<title></title>
	<meta name="description" content="">
	
	<!-- Icon -->
	<link rel="shortcut icon" href="images/favicon.ico">
	<link rel="apple-touch-icon" href="images/apple-touch-icon.png">
	
	
<!-- Mini CSS Reset -->
<link rel="stylesheet" href="css/css-mini-reset.css" type="text/css" />
	
<!-- Mobile -->
<link rel="stylesheet" type="text/css" href="css/mobile.css" media="only screen and (max-device-width: 480px)" />

<!-- Tablet pc -->
<link rel="stylesheet" type="text/css" href="css/tablet.css" media="screen and (min-device-width: 481px) and (max-device-width: 799px)"  />

<!-- Big screen -->
<link rel="stylesheet" type="text/css" href="css/main.css" media="screen and (min-device-width: 800px)" />

<!-- Print -->
<link rel="stylesheet" href="css/print.css" type="text/css" media="print" charset="utf-8">

<!-- If is lower then IE9  -->
<!--[if lt IE 9]>
<link rel="stylesheet" type="text/css" href="css/main.css" media="all"  />
<![endif]-->



  </head>
  <body>
    <header>
     <hgroup>
        <h1>Page Title</h1>
        <h2>Page Subtitle</h2>
      </hgroup>
    </header>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Archives</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
    <section>
      <article>
        <header>
          <h2><a href="#">Title</a></h2>
        </header>
        <section>
          <p>Lorem ipsum...</p>
        </section>
      </article>
      <article>
        <header>
          <h2><a href="#">Title</a></h2>
        </header>
        <section>
          <p>Lorem ipsum...</p>
        </section>
      </article>
      <article>
        <header>
          <h2><a href="#">Title</a></h2>
        </header>
        <section>
          <p>Lorem ipsum...</p>
        </section>
      </article>
    </section>
    <footer>
      <p>Content is licensed under a Creative Commons Public Domain License </p>
    </footer>
  </body>
</html>
```

# Action Button and next step of interaction

# Design Examples
[csszengarden.com](http://www.csszengarden.com/)
# Best Practices
[Frontend Checklist](https://frontendchecklist.io/)
[HTML-reset](https://github.com/charlesfinney/HTML5-Reset)
[HTML 5 Doctor](http://html5doctor.com/)

# Website Hosting
1. setup a digitalOcean Droplet
1. register a doman name at [ionos.com](https://www.ionos.com/domains/domain-names)
1. Then 
[point domain name to digitalOcean droplet](https://www.digitalocean.com/community/tutorials/how-to-point-to-digitalocean-nameservers-from-common-domain-registrars) 








