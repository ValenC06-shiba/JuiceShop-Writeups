# JuiceShop-Writeups
Repository where I explain on OWASP's JuiceShop challenges as best as I can :3

"OWASP Juice Shop is probably the most modern and sophisticated insecure web application! It can be used in security trainings, awareness demos, CTFs and as a guinea pig for security tools! Juice Shop encompasses vulnerabilities from the entire OWASP Top Ten along with many other security flaws found in real-world applications!" 

As the main description from OWASP themselves, Juice Shop is a playing ground for security enthusiasts alike to test their knowledge on Web Application Security. Their main page can be found on https://owasp.org/www-project-juice-shop/

To get started we first need to install the software:

Getting in to the main page of the website, we can see on the right a section for installation where you can choose the installation method you prefer.

To install, simply follow the steps detailed in their GitHub page at: https://github.com/juice-shop/juice-shop#from-sources

For me, I cloned directly from their github into my kali vm but you can choose to install their docker version as well.

After installation, to access JuiceShop on default setting,  go to any browser on your machine and go to localhost:3000.

Now we have a vulnerable web application running on our local host where we can try all sorts of exploits on.


"The application contains a vast number of hacking challenges of varying difficulty where the user is supposed to exploit the underlying vulnerabilities. The hacking progress is tracked on a score board. Finding this score board is actually one of the (easy) challenges!"

So from the main page of JuiceShop, we can see that they implemented a scoreboard to track challenges but we first need to find it, after finding the score board we can start on solving the challenges.
