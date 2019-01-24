---
published: true
layout: post
title: Understanding Server-Sent Events (SSE) As Part Of The API Landscape
date: 2017-12-20T09:00:00.000Z
tags:
  - API Evangelist
  - Real Time
  - Server-Sent Events
  - Streaming
  - Standards
image: >-
  https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories/server-racks-clouds_clean_view.jpg
---
<p><img src="https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories/server-racks-clouds_clean_view.jpg" align="right" width="45%" style="padding: 15px;" /></p>I'm continuing to break down the technology stack as I get to know [my new partner Streamdata.io](http://streamdata.io). Yesterday [I wrote about their use of JSON Patch for returning partial responses of changes made to an API that has been proxied through the service](http://apievangelist.com/2017/12/19/javascript-object-notation-json-patch/), and today I want to focus on understanding [Server-Sent Events (SSE)](https://en.wikipedia.org/wiki/Server-sent_events), which Streamdata.io uses to stream those events in real time to any consumer. In my experience, SSE is a lesser known of the real time technologies out there, but is one that holds a lot of potential, so I wanted to spend some time covering it here on the blog.

As opposed to technology that delivers a two-way stream, Server-sent events (SSE) is all about a client receiving automatic updates from a server via HTTP connection. The technology is a standard, with the Server-sent events (SSE) EventSource API being standardized as part of the HTML5 specification out of the W3C. Similar to Streamdata.io's usage of JSON Patch, SSE is all about efficiency. Making web APIs real time isn't always about having a two-way connection, and SEE is a great way to make things streaming in a one-way direction, only sending you what has changed in real-time using JSON Patch. Efficiency in direction, delivery, and in message.

Server-sent events (SSE) definitely shines when you look at how it can be used to constantly push and refresh data in any web UI using JavaScript. It's HTML5 roots makes it a first-class citizen in the browser, but I also think there are a huge number of scenarios to play with when it comes to system integration, and reducing polling on APIs. I think the news, currency, stock, and other financial data scenarios are the low hanging fruit, but I feel like Streamdata.io as a rapid deploy proxy that developers can throw in between any API and a system integration is where the killer use cases of Server-sent events (SSE) could be.

To help me validate this theory I will keep playing with [Streamdata.io](http://streamdata.io) and proxying any API I can get my hand on to see what is possible when you replace basic web API requests and responses with Server-sent events (SSE), and begin streaming only what changes after that initial request. I'm guessing that a whole new world of events will begin to emerge, allowing us to think about look at common web API resources differently. I feel like there is a lot of opportunity in deploying real-time, event-driven solutions like Kafka, and other Apache solutions, but I feel like there will be even more opportunity when it comes to getting intimate with the events that are already occurring across existing web APIs, even if the providers are fully tuned into what is going on, or have the resources to tackle event-driven architecture yet.

_**Disclosure:** [Streamdata.io](http://streamdata.io) is an API Evangelist partner._
