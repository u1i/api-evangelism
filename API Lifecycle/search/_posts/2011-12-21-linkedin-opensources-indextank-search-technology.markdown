---
title: LinkedIn Open-Sources IndexTank Search Technology
date: 2011-12-21 00:00:00 Z
tags:
- Search
layout: post
---

<a target="_blank"><img style="padding: 15px;" src="http://kinlane-productions.s3.amazonaws.com/linkedin/LinkedIn-Developer-Network.png" alt="" width="175" align="right" /></a><a title="LinkedIn has just open-sourced the technology behind IndexTank" href="http://engineering.linkedin.com/open-source/indextank-now-open-source">LinkedIn has just open-sourced the technology behind IndexTank</a> under the Apache 2.0 License.
<p></p>
The IndexTank technology has three separate toolsets:
<ul class="mainlist">
	<li><strong>IndexEngine</strong> - A real-time fulltext search-and-indexing system designed to separate relevance signals from document text</li>
	<li><strong>API</strong> - A RESTful interface that handles authentication, validation, and communication with the IndexEngine(s)</li>
	<li><strong>Nebulizer</strong> - Multitenant framework to host and manage an unlimited number of indexes running over a layer of Infrastructure-as-a-Service</li>
</ul>
<a href="http://indextank.com/" target="_blank"><img style="padding: 15px;" src="http://kinlane-productions.s3.amazonaws.com/api-evangelist/indextank/indextank_logo.png" alt="" width="250" align="right" /></a> An example of IndexTank in action is, Reddit, which runs on IndexEngine and the API.
<p></p>
They have the <a href="https://github.com/linkedin/indextank-engine">IndexTank Engine</a> and <a href="https://github.com/linkedin/indextank-service">IndexTank Service</a> code published at Github, and created a <a title="LinkedIn Group to Support It" href="http://www.linkedin.com/groups?gid=4224441">LinkedIn Group to support it</a>.