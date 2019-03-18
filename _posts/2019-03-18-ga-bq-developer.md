---
title: Things you need to know about BigQuery
date: 2019-03-18 
description: BigQuery is a tool that allows you to store, query, and extract data. It's a separate tool from GA and GTM, part of Google's Cloud Platform.
#image: "/img/measurement-in-mutli-screen-world5.jpg"
categories:
-  BigQuery
---

BigQuery is Google "managed" data warehouse for analytics that allows you to store, query, and extract data. It's a separate tool from Google Analytics and Google Tag Manager, and it is part of Google Cloud Platform.

BigQuery is a "managed data warehouse".  It allows you make a cheese sandwich (i.e. data warehouse) and you don't have to milk the cow, operate the mill or harvest the wheat or drive the Tractor.

![](https://camo.githubusercontent.com/b00c9c4e06a58ddf265b5ff4a45ea123c4c6f8c0/68747470733a2f2f7062732e7477696d672e636f6d2f6d656469612f44743844634c5f58634141686e56552e6a7067)

BigQuery has a free tier plan which allows you to query 1 Terabyte per month and store 10 gigabytes. With Google Analytics 360,  BigQuery is free, up to $500/month of usage. For website with over one-billion hits per month, that in the region of $150 per month for storage and $100 per month for querying. Google Analytics 360 customers benefit from a native integration with Google BigQuery. However, use of BigQuery is not restricted for Google Analytics 360 customers alone.
It just a little more involved to integrate the free Google Analytics with BigQuery. 

Why exports Google Analytics to BigQuery? 
- No more data sampling! This is a step-up for those sites having heavy traffic daily 
- An opportunity to build ANY reports with ANY segments using ANY configuration you like

If you need help on this, DM me.


This is what I learned so far after completing the course [From Data to Insights with Google Cloud Platform](https://www.coursera.org/account/accomplishments/specialization/PKU7C2X2QRG8)

- Do not use `SELECT * FROM report.all.*` on BigQuery. Such query would quickly blow out the 1TB free quota! Drill down the data table as it is much cheaper to query in terms of quota usage and execution time.

- The most common error using BigQuery `Cannot access field type on a value with type ARRAY<STRUCT<type STRING, amount INT64>` The correct way is add in the appropriate UNNEST( ) and WHERE Clause filter

![](https://pbs.twimg.com/media/DzXs3vFWkAAFcWK.jpg)

-  GA360 exports to BigQuery is specific to the view.  This means that anything you filter out in the view you’re exporting does not appear in the BigQuery data.	


