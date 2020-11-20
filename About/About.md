# About Priveasy

### Table of Contents

- [Overview](#overview "Overview")
- [Services](#services "Services")
  - [Web Application](#web-application "Web Application")
  - [VPN](#vpn "VPN")
  - [Burner Email](#burner-email "Burner Email")
  - [Burner Text Messaging](#burner-text-messaging "Burner Text Messaging")
  - [URL Shortener](#url-shortener "URL Shortener")
  - [Pastebin](#pastebin "Pastebin")
- [History](#history "History")
  - [Priveasy v0.0](#priveasy-v00 "Priveasy v0.0")
  - [Priveasy v1.0](#priveasy-v10 "Priveasy v1.0")
  - [Priveasy v1.x](#priveasy-v1x "Priveasy v1.x")
  - [Priveasy v2.0](#priveasy-v20 "Priveasy v2.0")
  - [Priveasy v3.0](#priveasy-v30 "Priveasy v3.0")
- [Administration](#administration "Administration")
- [Roadmap](#roadmap "Roadmap")

## Overview

Priveasy is the world's first (and only) Internet Privacy Services Provider (IPSP) that is both community-driven, and 100% open source. Our entire codebase is available online for anyone to inspect, improve upon, criticize, or contribute-to, making us the only truly, end-to-end transparent IPSP.

Priveasy is not an company, we are simply a not for profit collaborative: a growing community of dedicated developers who have come together to build something special, something from which everyone can benefit. While Priveasy does have an organizational structure, it is based solely on contributions, and allows anyone to rise or fall as time goes on, based on the level of commitment they are able to sustain.

Anyone is welcome to use Priveasy's services. Our goal is to guard everyone's rights to privacy and free speech at all times, no matter your place of origin, economic status, gender, race, sexual orientation, technical knowledge, etc. We are built by everyone to serve everyone.

Although it is true that Priveasy charges its users for plans, we do not take any profit. All of our expenditures are meticulously documented, and 100% of the money goes right back into providing our services. That is why we are able to provide our services at such low costs: we have almost no overhead, no greedy executives, and many, wonderful supporters and contributors.

At no point will you find any trackers, cookies, analytics, etc. on our website or embedded in our services. Priveasy takes your privacy seriously, and will go to great lengths to protect it. Don't believe us? Continue reading! You have access to our entire codebase right here at your fingertips. You will never find a single piece of code running on our servers that is not open source, and readily available for you to inspect.

## Services

### Web Application

##### Details (Features; Benefits; Uses):

- Our website is truly dedicated to user privacy. Unlike nearly every other website out there (including those of major VPN providers, who claim to guard your privacy), our website does not use any sort of 3rd. party analytics, trackers, cookies, etc.
- We use an audited, state of the art authentication backend to ensure the confidentiality of our users' data. We use Argon2 to hash users' passwords, which is universally considered to be the best and most secure.
- Our website enables HSTS.
- Our website is also available as an onion service (with the onion location header enabled).
- We're built with [Django](https://www.djangoproject.com/ "Django") which comes with a whole host of security assurances (for example, mandatory cross-site request forgery tokens).
- We accept payments in privacy coins, such as Zcash.
- Any inactive accounts (accounts without an active plan and which have not been logged-in to for a period of 30 days or more) are automatically deleted, along with all their associated data.

### VPN

##### Details (Features; Benefits; Uses):

- Encrypts all of your internet traffic (including DNS queries, even after they leave our servers).
- Prevents your network administrator, ISP, government, etc. from easily logging your browsing activities, and blocking specific sites or services.
  - Note: You should never use a VPN with the goal of becoming anonymous. VPNs do not make you truly anonymous, especially against a state-sponsored organization. If you are looking for anonymity, then [Tor](https://www.torproject.org/ "Tor") will take you farther than a VPN will.
- We have no access to any form of VPN logs.
- We offer a shadowsocks proxy (with optional v2ray plugin), allowing people in oppressive/restrictive countries/locations to safely and discretely access the open internet
- The main VPN protocol we use is WireGuard. WireGuard is known for being fast, secure, and open source, and is built right into the Linux kernel.
  - Our implementation of WireGuard takes advantage of its preshared key (PSK) functionality, meaning that your traffic is both symmetrically and asymmetrically encrypted, adding quantum resistance.
- Every user is reserved their own, private LAN, allowing their connected devices to communicate with each other locally, as if they were all connected to the same, home network.
- We have no hardcoded bandwidth or traffic limitations

### Burner Email

##### Details (Features; Benefits; Uses):

- We offer both burner email forwarding, and burner email sending.
  - Our burner email forwarding feature allocates you a whole bunch of "burner" email addresses, at our domain. A forwarding address is of the format: `example@fwd.priveasy.org`. This forwarding address will forward any email sent to it, to the "recipient" email address that you configure within your account. This allows you to give out our email address instead of your own, while still receiving any emails sent to it as if they were sent directly to your normal inbox. Should the person/company you gave our email to get hacked, sell your information, or start spamming you, you can simply delete the forwarder from your account, and have peace of mind.
  - Our burner email sending follows the same principles as the burner email forwarding service: it allows you to send email from a "burner" email account, other than your own. Sent burner emails can take either of the following formats: `example@fwd.priveasy.org` or `example@burn.priveasy.org`.
- The Priveasy servers in charge of handling burner email sending and receiving are specifically set up using postfix virtual aliases. What does this mean? It means that no matter what, whether you are sending an email or one is being forwarded to you, the contents of that email will never touch our hard drives.

### Burner Text Messaging

##### Details (Features; Benefits; Uses):

- We offer burner text message sending. This service allows you to send a text message to whomever you desire, from our phone number, instead of your own.
  - Please note: We have to use a 3rd-party service to send text messages. However, that 3rd-party does not get any access whatsoever to your account information.

### URL Shortener

##### Details (Features; Benefits; Uses):

- Our URL shortener allows you to take large URLs, and reduce them to the size of our domain name: Priveasy.org (12 characters). A shortened URL takes the form: `P5.vc/short`. You can then share this URL, and see from your dashboard how many times it was clicked. If at any point you don't want the destination to be accessible anymore, you can simply delete the shortener from your dashboard.

### Pastebin

##### Details (Features; Benefits; Uses):

- We offer a pastebin so you can quickly and easily save notes, code snippets, or any other important data. All pastes are saved privately by default, but come with the option to share them publicly, should you desire to do so.

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

By far, Priveasy v2.0 brought the largest changes ever made to Priveasy. Although at the time, at least to the users, it may not have seemed like it: there were major changes to the website, but the same general structure of the site and the main services it offered were retained. However, the entire backend was rewritten from scratch.

It had been clear for awhile that Priveasy's backend needed rewriting. It was extremely inefficient, slow, and overflowing with patch jobs to keep it technically functional, albeit poorly written. It wasn't until two major events occurred, however, that it was finally decided to scrap the backend and start over.

The first major problem was with [Algo VPN](https://github.com/trailofbits/algo "Algo VPN"). Although great for small projects, it did not scale well. While working on rewriting and customizing the code to be more functional/optimized for Priveasy, flaw after flaw kept appearing. Algo was extremely bloated, introducing a massive amount of overhead that Priveasy did not want to have to take on (to no fault of Algo: Priveasy simply wasn't interested in providing all the same features as Algo). It also revealed itself to be somewhat patchwork: the exact thing that Priveasy was trying to correct. Finally, utilizing Algo with more than a few dozen clients was not realistic at all. It was found out the hard way that Algo's IP address allocation and firewall rules quickly break down—without any warning—when a certain number of clients is reached. Again, this is in no way Algo's fault: it's only meant for personal servers, not for servers looking to maintain many different profiles. However, it was apparent that a custom solution would be required.

The second major problem was more general. Priveasy was looking into buying the rights to an extremely short URL, to use for a new privacy service. However, the backend, as it was written, only updated once every three hours: no one would want to have to wait three hours after generating a shortened URL, to use it. As a matter of fact, this problem applied to all of our other services: no one would want to wait 24 hours to be able to download their VPN credentials after paying for them; no one would want to wait three hours for the email forwarder they created to start working, etc. Therefore, the task of rewriting the backend to properly utilize a powerful database was undertaken.

Because all of the changes being made required modifying almost everything, the decision was made to start afresh, and rebuild from scratch. A new repository was initialized on `Monday, March 23, 2020 1:29:43 AM GMT-04:00 DST`, and Priveasy started over. Once the base rebuild was done, the first few commits were made, and Priveasy 2.0 was officially in production.

###### Log of major commits made to Priveasy v1.x:

```
0000000000000000000000000000000000000000 cb9b4d657e893b4c021d48b568e79713298567fc nonroot <Email Address Witheld> 1584941383 -0400	commit (initial): Initial Priveasy Commit
cb9b4d657e893b4c021d48b568e79713298567fc 2423c4123a16a16a2965b8399eebd0f191eda7ac unknown <Email Address Witheld> 1586383103 -0400	commit: Website Shell Added
2423c4123a16a16a2965b8399eebd0f191eda7ac 7546be3732eda744bad80cbf648a3ced0727c999 unknown <Email Address Witheld> 1589332153 -0400	commit: Website Fully Functional; Initial Public State
7546be3732eda744bad80cbf648a3ced0727c999 5ea654798fa358b717164424b1ae8db691196007 unknown <Email Address Witheld> 1589857526 -0400	commit: Added Legal Documentation and Support for Discount Codes
5ea654798fa358b717164424b1ae8db691196007 7a358c1523834e2eac1c74d6388b7339257d5e87 unknown <Email Address Witheld> 1589930482 -0400	commit: Bug Fix
7a358c1523834e2eac1c74d6388b7339257d5e87 96996645e17783b5c9f48080a64ae5b02d535164 unknown <Email Address Witheld> 1590444234 -0400	commit: Added Professional Email and Updated Admin Site (Added Budget Calculator)
96996645e17783b5c9f48080a64ae5b02d535164 36dd8619f7a9107dad23d3d37a33f962f092e1a6 unknown <Email Address Witheld> 1590548950 -0400	commit: Added HTML, Branded Emails
36dd8619f7a9107dad23d3d37a33f962f092e1a6 a47469545de584a3f5d242815da13d8afa68e718 unknown <Email Address Witheld> 1591081721 -0400	commit: Added Records/Email Server & Bug Fixes
a47469545de584a3f5d242815da13d8afa68e718 d336f4489d779c020f5d8f931b570a225211e778 unknown <Email Address Witheld> 1591122354 -0400	commit: Added Improved Email Functionality
d336f4489d779c020f5d8f931b570a225211e778 722efd069a9c192cf091c3008d913f0ce91f3eaf unknown <Email Address Witheld> 1591825646 -0400	commit: Complete VPN Overhaul
722efd069a9c192cf091c3008d913f0ce91f3eaf 99b0eeed3b152f8614167c2c99442ccb472f0d54 unknown <Email Address Witheld> 1592207850 -0400	commit: Custom 404 Page
99b0eeed3b152f8614167c2c99442ccb472f0d54 552c26ca5631d0492f9a739fd824477aa795ea9e unknown <Email Address Witheld> 1592209658 -0400	commit: Extended Page View Stats
552c26ca5631d0492f9a739fd824477aa795ea9e eb04b70605865803c754ddffe394f27a6fb004eb unknown <Email Address Witheld> 1592966405 -0400	commit: Add Social Media Creds, Enable Hidden Service Over HTTP, & Other Minor Changes
eb04b70605865803c754ddffe394f27a6fb004eb 37a9d0940d745fce6b7ec3accb85ff1f7f6c1927 unknown <Email Address Witheld> 1593076107 -0400	commit: Converted Line Endings (Default Changed From CRLF to LF)
37a9d0940d745fce6b7ec3accb85ff1f7f6c1927 7b331d6f481a9f40397e8f3713edd2f74bb939a8 unknown <Email Address Witheld> 1593076136 -0400	commit: Made Payment Settings Page Easier to Access
7b331d6f481a9f40397e8f3713edd2f74bb939a8 a6e1e8c42099d1fad282d643dccba3a935ab93d0 unknown <Email Address Witheld> 1594061840 -0400	commit: Added Support for Accepting Payments in Zcash
a6e1e8c42099d1fad282d643dccba3a935ab93d0 e8535697a595e6cb8e45a97f24c2fb0162d549f5 unknown <Email Address Witheld> 1594170412 -0400	commit: Fixed alignment/text bugs on account page
e8535697a595e6cb8e45a97f24c2fb0162d549f5 a61d97ede5eb170d61b39142ee60ef9919d56a2e unknown <Email Address Witheld> 1594247081 -0400	commit: Added QR codes to cryptopayment page, as well as view stats
a61d97ede5eb170d61b39142ee60ef9919d56a2e ff86216475bfb76ee5bb72d4ad11a8508b196253 unknown <Email Address Witheld> 1594268175 -0400	commit: Added payment amount estimates on cryptopayment page, username case insensitivity, and further Zcash payment checks
ff86216475bfb76ee5bb72d4ad11a8508b196253 fe157c1f0e09ec7654931bb9c87344d911a9b63d unknown <Email Address Witheld> 1595040360 -0400	commit: Added Onion-Location header and more credentials
```

### Priveasy v3.0

Priveasy v3.0's story has not yet been told. Priveasy v3.0 is by far the most ambitious project in the history of Priveasy. Priveasy v3.0 is when we dedicate ourselves to the good of humanity, and come together to build a community, and write history together. Priveasy v3.0 is when I take all of my precious code, all of my hard work, and lay it bare, for the world to see. Priveasy v3.0 is when we acquire our own servers, and work together to build something bigger than us all. Priveasy v3.0 is still in the works, but when it's done, it will be historic.

## Administration

> This section provides an overview of the administrative aspects of Priveasy. For transparency and trust reasons, we felt that it was important to include this section. However, we cannot provide every detail here, in order to protect the identities of those invested in our cause who wish to remain private, as well as other sensitive information such as our exact server locations. If you would like access to greater information, please contact us directly.

> Please note: major contributors to Priveasy (people who have worked with us for awhile yet are not directly affiliated with us or part of our core team) are given access to this extra information by default. This allows us to have third parties who are active and trusted by the open source community vouch for us, and our administrative process. If you would like to be one of these third parties, you are more than welcome to start contributing to our code, and we'd love to have you! If for any reason you think that you have been contributing to us for awhile, and we've accidentally overlooked you, please reach out and let us know!

Priveasy is currently run as not for profit organization. We have a few people dedicated to our cause who handle the administrative aspects of Priveasy, as well as maintain consistent development.

Priveasy currently calculates its price per plan by taking the exact amount it costs us to run these services, multiplying that amount by 1.5, and then dividing the final amount by the number of users we have.

The extra 50% we take goes towards paying our developers and administrative staff, advertising, getting third party security audits, covering legal fees, maintaining bug bounties, etc. As Priveasy grows and we gain more users, we plan to lower this percentage significantly.

Priveasy is looking to transition to a transparent financial system, such as that provided by Open Collective. However, we have been informed that we may not do so until we reach 100 stars on GitHub. As such, if you are reading this, please star our repositories, as you'll be directly helping us to become even more transparent. Thank you!

## Roadmap

### An outline of current goals and planned additions to Priveasy

#### Ordered, technical, and short-term goals:

1. Verify email accounts/forwarders via a link (remove/modify the need to enter a long token)
1. Require email account verification upon sign up
1. Add 2FA
1. Encrypt all pastes by default (or at the very least optionally) with secrets inaccessible to Priveasy
1. Implement BotBlock in an efficient fashion (that doesn't significantly strengthen the effects of a DDoS)
1. Add support for reserved burner phone numbers (to allow for text message sending and receiving/forwarding)

#### General, non-ordered, or long-term goals:

- Work on building a stronger community of users, contributors, supporters, sponsors, influencers, etc.
- Consider removing the need to ask for a user's first name
- Look into autodetecting abuse on VPN servers, and auto ban/rate limit those accounts (with all analysis/actions done solely on the VPN server, to preserve privacy)
- Develop a Priveasy mobile application
- Crowdfund to acquire our own, physical servers, instead of renting VPS's from 3rd-party hosting providers
