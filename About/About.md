# About Priveasy

### Table of Contents

- [Overview](#overview "Overview")
- [History](#history "History")
  - [Priveasy v0.0](#priveasy-v00 "Priveasy v0.0")
  - [Priveasy v1.0](#priveasy-v10 "Priveasy v1.0")
  - [Priveasy v1.x](#priveasy-v1x "Priveasy v1.x")
  - [Priveasy v2.0](#priveasy-v20 "Priveasy v2.0")
  - [Priveasy v3.0](priveasy-v30 "Priveasy v3.0")
- [Services](#services "Services")
- [Goals](#goals "Goals")

## Overview

Priveasy is the world's first (and only) Internet Privacy Services Provider (IPSP) that is both community-driven, and 100% open source. Our entire codebase is available online for anyone to inspect, improve upon, criticize, or contribute-to, making us the only truly, end-to-end transparent IPSP.

Priveasy is not an company, nor a non-profit. We are simply a collaborative: a growing community of dedicated developers who have come together to build something special, something from which everyone can benefit. While Priveasy does have an organizational structure, it is based solely on contributions, and allows anyone to rise or fall as time goes on, based on the level of commitment they are able to sustain.

Anyone is welcome to use Priveasy's services. Our goal is to guard everyone's rights to privacy and free speech at all times, no matter your place of origin, economic status, gender, race, sexual orientation, technical knowledge, etc. We are built by everyone to serve everyone.

Although it is true that Priveasy charges its users for plans, we do not take any profit. All of our expenditures are meticulously documented, and 100% of the money goes right back into providing our services. That is why we are able to provide our services at such low costs: we have almost no overhead, no greedy executives, and many, wonderful supporters and contributors.

At no point will you find any trackers, cookies, analytics, etc. on our website or embedded in our services. Priveasy takes your privacy seriously, and will go to great lengths to protect it. Don't believe us? Continue reading! You have access to our entire codebase right here at your fingertips. You will never find a single piece of code running on our servers that is not open source, and readily available for you to inspect.

## History

### Priveasy v0.0

Although Priveasy may not have gotten a website or even its name until May of 2019, it was in the works long beforehand. Years before its official creation, Priveasy's founder—Noah—had dedicated his life to internet privacy and security. He was active in the open source community, contributing to many projects, and creating many more of his own. But, it wasn't until he entered high school that Priveasy really started to take shape. Concerned with the extensive levels of logging/tracking/blocking being done by the school system, the town's ISP, and even the federal government, Noah made it his goal to create a solution. Before long, he stumbled across [Algo VPN](https://github.com/trailofbits/algo "Algo VPN"), and used it to set up a simple VPN server for he and his classmates to use. A short while later, there was a long list of users, whom he charged $0.30 each per month, to help cover the server costs.

Although Noah was happy with the VPN server, it still wasn't enough for him, and his "client" list was only growing. It was around this time that he began researching and drafting other important privacy tools to implement, as well as a way to make those services scalable, and automated. And that, is how Priveasy was born.

### Priveasy v1.0

Many events and lots of work lead up to the formation of Priveasy.org, but I think it's safe to say that the creation of the actual website itself didn't begin until May of 2019, with the official domain name being registered on June 8, 2019.

This first version of the website was extremely simple, to say the least. Most of the work went into the backend, and it took months to develop. The original site consisted of only three services: a VPN, a burner email forwarder/sender, and a pastebin. The VPN was still run with [Algo VPN](https://github.com/trailofbits/algo "Algo VPN") (just automated), the email services were achieved with a simple [postfix](https://github.com/vdukhovni/postfix "postfix") setup, and the pastebin saved pastes by dumping them all into a single database entry. The website itself used basic bootstrap templates, and was nothing flashy. Overall, the site was slow (updating public pastes, email forwarders, etc. only once every 3 hours, and creating VPN profiles only once every 24 hours). But, despite its downfalls, the site served its purpose, and provided an excellent base to build upon.

###### Priveasy v1.0's Home Page:

![The top of Priveasy v1.0's home page](https://raw.githubusercontent.com/P5vc/Documentation/master/About/homePageTop.PNG "The top of Priveasy v1.0's home page")

![The middle of Priveasy v1.0's home page](https://raw.githubusercontent.com/P5vc/Documentation/master/About/homePageMiddle.PNG "The middle of Priveasy v1.0's home page")

###### Priveasy v1.0's Account Page:
![Priveasy v1.0's account page](https://raw.githubusercontent.com/P5vc/Documentation/master/About/accountPage.PNG "Priveasy v1.0's account page")

### Priveasy v1.x

After Priveasy's initial public release in June, a lot of work went into debugging the site, researching new features, and working around a myriad of problems that arose. Soon enough, it was abundantly clear that some form of version control was needed. On `Friday, October 25, 2019 9:17:45 PM GMT-04:00 DST`, about six months after the public release, the first-ever commit was made.

This first commit wasn't made until a massive amount of effort was put into the functionality of the backend, and into the squashing of bugs. The hope was to use this first commit to document the "initial" state of Priveasy, before doing a complete overhaul to the webdesign. However, over time, many other features were added and changes were made.

###### Log of major commits made to Priveasy v1.x:

```
0000000000000000000000000000000000000000 1c840c32674b4fc2f20694911bd5eb08c25fa178 nonroot <Email Address Witheld> 1572052665 -0400	commit (initial): Initial commit. Decided to start using version control while developing Priveasy. This initial commit contains all of the functional code written up to this point, for the website and its services.
1c840c32674b4fc2f20694911bd5eb08c25fa178 d742380c0efcce2d94dbd7e567a166002dd66b74 unknown <Email Address Witheld> 1572128962 -0400	commit: Added the updated home.html file and supporting files from after the redesign, and removed the designated login page, as logins are now handled directly from the home page.
d742380c0efcce2d94dbd7e567a166002dd66b74 cf97b56785f4d2c5504d0ea2514d25592a831588 unknown <Email Address Witheld> 1572143012 -0400	commit: Many small changes; Revamped Register Page
cf97b56785f4d2c5504d0ea2514d25592a831588 d5b655537ad5317253c72719423e11cf66539da1 unknown <Email Address Witheld> 1572143636 -0400	commit: Made Django Template Friendly
d5b655537ad5317253c72719423e11cf66539da1 3bfbd135f7727fd3f4c87577a8e16c5103da136f unknown <Email Address Witheld> 1572144335 -0400	commit: Added terms agreement
3bfbd135f7727fd3f4c87577a8e16c5103da136f 54b2fc8dff8564b260181fd3aecda12dbc151551 unknown <Email Address Witheld> 1572144955 -0400	commit: Update register section
54b2fc8dff8564b260181fd3aecda12dbc151551 be879d16608ec2f047892a19347fcbaafafd4482 unknown <Email Address Witheld> 1572146823 -0400	commit: Added a new image and spacing to the register page.
be879d16608ec2f047892a19347fcbaafafd4482 560c7bf5fb3267d20eb99897844d6cfee17b0243 unknown <Email Address Witheld> 1572147191 -0400	commit: Corrected Image Directory
560c7bf5fb3267d20eb99897844d6cfee17b0243 517177acfb8b562fe7365d932b01b720ed31c117 unknown <Email Address Witheld> 1572147426 -0400	commit: Corrected Image Filepath
517177acfb8b562fe7365d932b01b720ed31c117 30906cec3fa316e38ee0403e454bbe0819c5dee5 unknown <Email Address Witheld> 1572148812 -0400	commit: Add form error messages
30906cec3fa316e38ee0403e454bbe0819c5dee5 68a3663972bb1f5400b7c5069f16f44f4ddbc7c9 unknown <Email Address Witheld> 1572149560 -0400	commit: Make sure both passwords match; if they do not, raise an error
68a3663972bb1f5400b7c5069f16f44f4ddbc7c9 473bff1658fa4883f83250d4c575ef5e814913d8 unknown <Email Address Witheld> 1572149781 -0400	commit: Fixed syntax error
473bff1658fa4883f83250d4c575ef5e814913d8 f8083ece4a093678934233ec566e64cc23cd8784 unknown <Email Address Witheld> 1572150265 -0400	commit: Improved Form Error Handling
f8083ece4a093678934233ec566e64cc23cd8784 0e506494b5a2e45c9426cfd59221f4782338ad13 unknown <Email Address Witheld> 1572154644 -0400	commit: All of the register page bugs squashed; now fully functioning
0e506494b5a2e45c9426cfd59221f4782338ad13 1530500ed08b71674cffd975219a6df06cb928f7 unknown <Email Address Witheld> 1578970963 -0500	commit: Server migration update
1530500ed08b71674cffd975219a6df06cb928f7 042a815a19f91b69d5cc70e37418a8617a00f684 unknown <Email Address Witheld> 1579466875 -0500	commit: Major changes. Too many to list!
042a815a19f91b69d5cc70e37418a8617a00f684 e96efc583c93eccf1d89eb4bb1c66a18d5de7af1 unknown <Email Address Witheld> 1579478612 -0500	commit: Enhanced VPN download notifications
e96efc583c93eccf1d89eb4bb1c66a18d5de7af1 afeee4cc547f02ae0d8bb1df05a1ff72e2a5df60 unknown <Email Address Witheld> 1579588952 -0500	commit: Installation instructions for VPN, fixed major VPN server sync bug, etc.
afeee4cc547f02ae0d8bb1df05a1ff72e2a5df60 fcf9db500fc9746150f4742b4ea0ab15ec78456f unknown <Email Address Witheld> 1579661791 -0500	commit: Added acceptable use message.
fcf9db500fc9746150f4742b4ea0ab15ec78456f cccb99ba6f947f21ce2b47062206fbd7944f93ae unknown <Email Address Witheld> 1579903613 -0500	commit: Add network statistics to email report
cccb99ba6f947f21ce2b47062206fbd7944f93ae cf9ce0826a730f8286e6d5814e2378ad73d9ffee unknown <Email Address Witheld> 1582694654 -0500	commit: Support for tor, cryptocurrencies, new logo, and much, much more! (views.py changes witheld until later date)
cf9ce0826a730f8286e6d5814e2378ad73d9ffee d6d805c8f795266f5640b179a028eea14e2566b9 unknown <Email Address Witheld> 1582777689 -0500	commit: Referral Code Updates & Bug Fixes
d6d805c8f795266f5640b179a028eea14e2566b9 2fc34e57100ab20a0d79bcdf44f408f44077b5d7 unknown <Email Address Witheld> 1582871341 -0500	commit: Major email update, usability update, and bug fixes
2fc34e57100ab20a0d79bcdf44f408f44077b5d7 13d91a26595bb1454bb41e4d99d10c74e4b7cf5b unknown <Email Address Witheld> 1583044823 -0500	commit: Added Text Messaging Support & Lowered Plan Prices
13d91a26595bb1454bb41e4d99d10c74e4b7cf5b 10a5e976106484bb0cc8433263b364449dd098b7 unknown <Email Address Witheld> 1583201762 -0500	commit: Texting updates & merch link added.
10a5e976106484bb0cc8433263b364449dd098b7 fa2c87f0487a8495caecfacb2060cff203c92412 unknown <Email Address Witheld> 1583306012 -0500	commit: Home page header redesign
```

###### Priveasy's home page after the redesign:

![Priveasy's redesigned home page](https://raw.githubusercontent.com/P5vc/Documentation/master/About/PriveasyV1xHomePage.PNG "Priveasy's redesigned home page")

### Priveasy v2.0



### Priveasy v3.0



## Services



## Goals

