# StateFarm
Files for review by State Farm hiring personnel

### Overview
This file was part of the IBM Design Principle Application that IBM ran last year- initially a PDF/paperwork based application. The changes over to digital not only helped secure the promotion, but also became the suggested standard for IBM promotion applications in order to cut down on paper waste and hiring mgmt eye strain. 

Of the code on the 'IBM' page, the page initiallizes and pulls the confirmation from the 'login' page to ensure the correct member is logged in. Then, all the structure and menus initialize. Of the content, much of it is hidden within expandable divs, which the content further broken down into sections preceded by a 'more' button, which exapnds the next piece of content. Only one main show/hide div may be open at one time. Interacting with one will automatically close and minimize each other show/hide div. On each page load, the URL is modified to reflect the page that is open. This URL is stored in an inline link variable, trimmed with javascript and then output to the URL. 

The submenus of white squares is handled by two CSS states that is switched between using javascript/jquery class switching on the hover eventHandler. As with other features, clicking an instance of the menu squares keeps it expanded and will minimize any other square buttons while also changing the content out to the correct set. 

All together this creates a very simple, elegant system that just handles the site needs without a large amount of backend code libraries other then some simple masonry for layout and then the latest remote file for JQuery. All images and relevant files have been web optimized for load speed. The entire site was created and launched within two months which included feedback and scheduling with client. 

### Main Site URL for reference
If further context is needed, the site in it's entireity is available at www.tropesites.com/IBMDPKallish/login.html utilizing the username of "ReviewApplication" and a password of "Rand29Noyes!5". This password is checked against the correct response using a simple PHP string comparison. The password is simply held inline rather then hosted in a seperate pw protected file as this application in its final form was hosted on the internal BlueMix IBM webspace, and was thus unlikely to have unauthorized access that would normally require a more robust password handling system. 
