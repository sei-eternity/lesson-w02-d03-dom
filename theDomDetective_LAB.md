# Lab: DOM Access

## DOM Detective

Open up [Girl Develop It](https://www.girldevelopit.com/) in Chrome or Firefox, and open up the JavaScript console (CMD + Option + J on Macs).

Use DOM access methods (e.g. `document.querySelector`) to find the following parts of the page. You probably first want to use Inspect Element to figure out what their tag names, classes, and IDs are.

- Every image on the page

document.querySelectorAll('img');


- The navigation area in the upper right
<!-- 
document.querySelectorAll('a href'); -->
document.querySelectorAll('.navigation')[0]

- The MailChimp sign-up form in the bottom
document.querySelector('input');

- The upper left-hand logo that says GDI (Hint: use CSS descendant selectors)
document.querySelector('.logo');

- The logos of the media sources that featured GirlDevelopIt (lifeHacker, TED, etc., at the bottom of the page)
document.querySelector('.press-logos');

- The big heading that says "DON'T BE SHY DEVELOP IT"

<!-- document.getElementsByClassName('animated fadeInLeft'); -->
document.querySelector('.opener');

- All of the headings that have the underline (e.g. Who we are, We are now in 63 cities)

document.querySelectorAll('h2');

- All of the images that are in the stats part of the page (e.g. 26%, 18% and 34%)

document.getElementsByClassName('stats');

- BONUS: all the dots in the map

document.querySelector('circle');
