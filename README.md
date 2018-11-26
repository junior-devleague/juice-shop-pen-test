# Juice Shop Hacking Guide

A walkthrough of the 1 star "Trivial Challenges" for the super vulnerable OWASP Juice Shop web application.

### Resources
* [Challenge Hunting - OWASP Official Hacking Guide](https://bkimminich.gitbooks.io/pwning-owasp-juice-shop/content/part2/)


### Challenges
1. Find the score board
    * Since we know the page exists, we can simply guess what the URL will be
    * `https://khs-juice-shop.herokuapp.com/#/score-board`
2. Find the admin page
    * Open the developer tools -> Source tab
    * Inspect the `main.js` file
    * `ctrl + f` and search for the word `admin`
        * ![juice-shop-administration-route](img/juice-shop-administration.png)