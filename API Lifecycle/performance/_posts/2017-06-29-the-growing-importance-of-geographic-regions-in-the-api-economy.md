---
published: true
layout: post
title: The Growing Importance of Geographic Regions In API Operations
date: 2017-06-29T16:00:00.000Z
tags:
  - API Evangelist
  - Regions
  - Deployment
  - International
  - Reliability
  - Performance
image: >-
  https://s3.amazonaws.com/kinlane-productions/3D-Printing/regions/api-regions-global-map-from-google.png
---
<p><a href="https://cloud.google.com/about/locations/"><img src="https://s3.amazonaws.com/kinlane-productions/3D-Printing/regions/api-regions-global-map-from-google.png" align="right" width="40%" style="padding: 15px;" /></a></p>I have been revisiting [my earlier work on an API rating system](http://apievangelist.com/2015/10/31/how-are-we-going-to-create-the-standard-and-poors-and-moodys-for-the-api-economy/). One area that keeps coming up as I'm working is around the availability of APIs in a variety of regions, and the cloud platforms that are driving them. [I have talked about regional availability of APIs](http://apievangelist.com/2011/02/04/launch-region-specific-apis/) for some time now, keeping an eye on [how API providers are supporting multiple regions](http://apievangelist.com/2016/01/05/your-api-access-replicated-into-multiple-regions-around-the-globe-for-additional-charge/), as well as [the expanding world of cloud computing](http://apievangelist.com/2017/05/08/regional-availability-when-it-comes-to-api-access/) that is powering these regional examples of providing and consuming APIs.  

I have been watching [Amazon rapidly expand their available regions](http://docs.aws.amazon.com/general/latest/gr/rande.html), as well as [Google](https://cloud.google.com/compute/docs/regions-zones/regions-zones) and [Microsoft](https://azure.microsoft.com/en-us/regions/) racing to catch up. But I am starting to see API providers [like Digital Ocean providing APIs for getting at geographic region information](https://developers.digitalocean.com/documentation/v2/#regions), and [Amazon provides API methods for getting the available regions for Amazon EC2 compute](http://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeRegions.html)--I will have to check if this is standard across all services. [Twilio has regions for their API client](https://www.twilio.com/docs/api/client/regions), and [Runscope has a region API for managing how you run API tests from a variety of regions](https://www.runscope.com/docs/api/regions). The role of geographic regions when it comes to providing APIs, as well as consuming APIs is increasingly part of the conversation when you visit the most mature API platforms, and something that keeps coming up on my radar.

We are still far from the average company being able to easily deploy, deprecate, and migrate APIs seamlessly across cloud providers and geographic regions, but as APIs become smaller and more modular, and cloud providers add more regions, and APIs to support automation around these regions, we will begin to see more decisions being made at deploy and run time regarding where you want to deploy or consume your API resources. To be able to do this we are going to need a lot more data and common schema regarding the what geographic regions are available for deployment, what services operate in which regions, and other key considerations about exactly where our resources should operate. This is why I'm revisiting this work, to see what I can do to get API service providers to share more data from either the API provider or consumer side of the equation.

I am considering adding an area of my research dedicated to API regions, aggregating examples of how geographic regions are playing a role in API operations. I'm thinking region availability will be playing just as significant role as [performance](http://performance.apievangelist.com), [plans](http://plans.apievangelist.com), [security](http://security.apievangelist.com), [reliability](http://reliablity.apievangelist.com), and other areas of the API lifecycle when it comes to deciding where you deploy or consume your APIs. It feels like another one of the aspects of API operations that will overlap with many stops along the API lifecycle--not just [deployment](http://deployment.apievangelist.com). One of the areas of the API lifecycle I'm increasingly thinking about that will affect geographic API decisions is [regulations](http://regulation.apievangelist.com), and how governments are dictating what is acceptable when it comes to the storage, transmission, and access of digital resources. It feels like early notions of what the World Wide Web has been for the last 25 years is about to be blown out of the water, with the influences of digital nationalism, regulation, or even the Internet moving off planet, and increasingly driven by satellite infrastructure.