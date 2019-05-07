---
title: Google Tag Manager (GTM) or gtag.js?
date: 2019-05-07 
description: Google Tag Manager (GTM) or gtag.js? 
#image: "/img/measurement-in-mutli-screen-world5.jpg"
categories:
-  GTM
---

Google Tag Manager is a robust and full-featured tag management system, which supports Google and 3rd party tags(Facebook conversion pixels or heatmapping tool tags). 

`gtag.js` is a script that works just like Google Tag Manager. `gtag.js` allows you to send data to only Google Marketing Platform (Google Ads, Campaign Manager, Display & Video 360, Search Ads 360, and Google Analytics) No other 3rd party tags such as Facebook conversion pixels or heatmapping tool tags

You just need one snippet per page.


Your gtag.js snippet would look like this if you’re using Google Analytics and Google AdWords together

 ~~~
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-1234567-8');
  gtag('config', 'AW-1234567-8');
</script>
 ~~~

For product-specific documentation related to gtag.js, refer to the following:

- [Google Analytics](https://developers.google.com/analytics/devguides/collection/gtagjs/)
- [Remarketing](https://support.google.com/google-ads/answer/2454000)
- [Google Ads conversions](https://support.google.com/google-ads/answer/1722022)
- [Campaign Manager and Display & Video 360 know also as DCM](https://support.google.com/dcm/partner/answer/7568534)
- [Search Ads 360](https://support.google.com/searchads/answer/7550511)

