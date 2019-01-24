---
published: true
layout: post
title: Five APIs to Guide You on Your Way to the Data Dark Side
date: 2018-01-17T14:00:00.000Z
tags:
  - API Evangelist
  - Data
  - Surveillance
  - Privacy
image: ''
---
<p><img src="https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories-new/76_135_800_500_0_max_0_1_-1.jpg" align="right" width="45%" style="padding: 15px;" /></p>I was integrating with [the Clearbit API](https://dashboard.clearbit.com/docs#api-reference), doing some enrichment of the API providers I track on, and I found their API stack pretty interesting. I'm just using the enrichment API, which allows me to pass it a URL, and it gives me back a bunch of intelligence on the organization behind. I've added a bookmarklet to my browser, which allows me to push it, and the enriched data goes directly into my CRM system. Delivering what it the title says it does--enrichment.

Next up, I'm going to be using the Clearbit Discovery API to find some potentially new companies who are doing APIs in specific industries. As I head over the to the docs for the API, I notice the other three APIs, and I feel like they reflect the five stages of transition to the data intelligence dark side.

- **Enrichment API** - The Enrichment API lets you look up person and company data based on an email or domain. For example, you could retrieve a person’s name, location and social handles from an email. Or you could lookup a company’s location, headcount or logo based on their domain name.
- **Discovery API** - The Discovery API lets you search for companies via specific criteria. For example, you could search for all companies with a specific funding, that use a certain technology, or that are similar to your existing customers.
- **Prospector API** - The Prospector API lets you fetch contacts and emails associated with a company, employment role, seniority, and job title.
- **Risk API** - The Risk API takes an email and IP and calculates an associated risk score. This is especially useful for figuring out whether incoming signups to your service are spam or legitimate, or whether a payment has a high chargeback risk.
- **Reveal API** - Reveal API takes an IP address, and returns the company associated with that IP. This is especially useful for de-anonymizing traffic on your website, analytics, and customizing landing pages for specific company verticals.

Your journey to the dark side begins innocently enough. You just want to know more about a handful of companies, and the data provided is a real time saver! Then you begin discovering new things, finding some amazing new companies, products, services, and insights. You are addicted. You begin prospecting full time, and actively working to find your latest fix. Then you begin to get paranoid, worried you can't trust anyone. I mean, if everyone is behaving like you, then you have to be on your guard. That visitor to your website might be your competitor, or worse! Who is it? I need to know everyone who comes to my site. Then in the darkest depths of your binges you are using the reveal API and surveilling all your users. You've crossed to the dark side. Your journey is complete.

Remember kids, this is all a very slippery slope. With great power comes great responsibility. One day you are a scrappy little startup, and the next your the fucking NSA. In all seriousness. I think their data intelligence stack is interesting. I do use the enrichment API, and will be using the discovery API. However, we do have to ask ourselves, do we want to be surveilling all our users and visitors. Do we want to be surveilled on every site we visit, and on every application we use? At some point we have to make sure and check how far towards the dark side we've gone, and ask ourselves, is this all really worth it?

_**P.S.** This story reminds me I totally flaked on delivering a white paper to Clearbit on the topic of risk. Last year was difficult for me, and I got swamped....sorry guys. Maybe I'll pick up the topic and send something your way. It is an interesting one, and I hope to have time at some point._
