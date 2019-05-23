---
title: Implications of PWAs for digital analytics
date: 2019-05-21
description:  Using Google Analytics and Google’s workbox library for PWA
image: "https://media.licdn.com/dms/image/C5612AQENkOHOOUZLWg/article-cover_image-shrink_720_1280/0?e=1564012800&v=beta&t=iPU8ADDXPmUsIIQBzlmnm_aWOMHGncx6tzSUQKwQLqg"
categories:
-  PWA
---


Progressive Web Apps (PWAs) are mobile websites designed to behave as similarly to a native app experience as possible. It offer functionality that replicate native apps, such as push notifications and offline access.

Unlike native apps on mobile - PWAs don’t require installation or updates to fix bugs or offer new features. As it is not a mobile native apps, it allows you to bypass Google Play or Apple App Store.

Try https://airhorner.com/ on your mobile

For business with limited resources, PWA is a boon for developer resources. You do not need to create a mobile native app for Android, iOS separately. PWAs are JavaScript-based apps, developers do not need to gain new skills, but rather learn the new APIs offered through the Service Workers (a JavaScript file)

The main draw of PWA is the added off-line support. Off-line support ensuring basic functionality will continue when network connectivity is poor or non-existent. This improve user experience but at the cost of the ability to track and measure those experience. This is a trade off not any data-driven team willing to make.

Google [workbox-google-analytics](https://developers.google.com/web/tools/workbox/modules/workbox-google-analytics) is a library that implements offline analytics using IndexedDB, a Web storage standard in all major browser. 

Using Google Analytics and Google’s workbox library, it’s just a matter of calling

`workbox.googleAnalytics.initialize();`


Given the different website architecture of PWA, here Google [documentation](https://developers.google.com/web/ilt/pwa/integrating-analytics#analytics_and_service_worker) on integrating Google Analytics and Service Worker.

## Useful Resources

If you want to be convinced the business benefits of PWA, this is the site. https://www.pwastats.com/

How the sausage is made https://developers.google.com/web/progressive-web-apps/

A directory of PWS out there from whimsical to real deal https://pwa-directory.appspot.com/


This article is first published on Linkedin at https://www.linkedin.com/pulse/implications-pwas-digital-analytics-yap-s-s/

