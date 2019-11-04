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

# Action Button and next step of interaction

# Design Examples

# Best Practices
[Frontend Checklist](https://frontendchecklist.io/)
[HTML-reset](https://github.com/charlesfinney/HTML5-Reset)

# Website Hosting
1. setup a digitalOcean Droplet
1. register a doman name at [ionos.com](https://www.ionos.com/domains/domain-names)
1. Then 
[point domain name to digitalOcean droplet](https://www.digitalocean.com/community/tutorials/how-to-point-to-digitalocean-nameservers-from-common-domain-registrars) 








