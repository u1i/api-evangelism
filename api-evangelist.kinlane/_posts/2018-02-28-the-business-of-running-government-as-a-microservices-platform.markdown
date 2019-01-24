---
published: true
layout: post
title: The Business of Running Government As A Microservices Platform
date: 2018-02-28T09:00:00.000Z
tags:
  - API Evangelist
  - Federal Government
  - State Government
  - County Government
  - City Government      
  - Government
  - Monetization
  - Plans
  - Microservices
image: >-
  https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories/capital-battle_blue_circuit.jpg
---
<p><img src="{{ page.image }}" width="45%" align="right" style="padding: 15px;" /></p>
I recently <a href="http://apievangelist.com/2018/02/24/department-of-veterans-affairs-lighthouse-platform-rfi-round-two/">wrote a response to a recent Department of Veterans Affairs RFI which contained a section about the business of operating government as a microservices platform</a>.I know that many folks wouldn't make it that far in the 10K word response, so I wanted to break it out into its own post. I feel pretty strongly about the potential of decoupling how we deliver technology across government, but for this to be successful we are also going to have to decouple the business and politics of it all as well. This post reflects <a href="http://public.data.api.management.apievangelist.com/">my current research and thinking about the business of APIs in government, and is part of some ongoing work I am doing around API management, public data, and how we begin to think differently about how government engages with the public in a digital age</a>.

There are many interpretations of what is a microservice, but for the purposes of this post, it is a simple set of APIs that meet one precise set of government services. The API definition, database, back-end code, management layer, documentation, support and all other essential elements are self-contained, and usually stored in a single Github, or Bitbucket repository, when delivering microservices. Each microservice possesses its own technical, business, and political contract, outline how the service will be delivered, managed, supported, communicated, and versioned. These contracts can be realized individually, or grouped together as a larger, aggregate contract that can be submitted, while still allowing each individual service within that contract to operate independently.

**Decoupling The Business Of Delivering Government Digital Services**
The microservices approach isn’t just about the technical components. It is about making the business of delivering vital government services more modular, portable, and scalable. Something that will also decouple and shift the politics of delivering critical services to veterans. Breaking things down into much more manageable chunks that can move forward independently at the contract level. Helping both simplify, and streamline the deliver of services for both the provider, vendor, as well as any other stakeholders involved in the software lifecycle. Microservices isn't just about decoupling the technology, it is about decoupling the business of delivering digital services:

- **Micro Procurement** - One of the benefits of breaking down services into small chunks, is that the money needed to deliver the service can become much smaller, potentially allowing for a much smaller, more liquid and flowing procurement cycle. Each service has a micro definition of the monetization involved with the service, which can be aggregated by groups of services and projects.
- **Micro Payments** - Payments for service deliver can be baked into the operations and life cycle of the service. API management excels at measuring how much a service is accessed, and testing, monitoring, logging, security, and other stops along the API life cycle can all be measured, and payments can be delivered depend on quality of service, as well as volume of service.

Amazon Web Services already has the model for defining, measuring, and billing for API consumption in this way. This is the bread and butter of the Amazon Web Services platform, and the cornerstone of what we know as the cloud. This approach to delivering, scaling, and ultimately billing or payment for the operation and consumption of resources, just needs to be realized within each agency, and the rest of the federal government. We have seen a shift in how government views the delivery and operation of technical resources using the cloud over the last five years, we just need to see the same shift for the business of APIs over the next five years.

**Changing The Way Government Does Business**
API management is where you begin changing the way government does business. API management has been used for a decade to measure, limit, and quantify the value being exchanged at the API level. Now that API management has been baked into the cloud, we are starting to see the approach being scaled to deliver at a marketplace level. With over ten years of experience with delivering, quantifying, metering and billing at the API level, Amazon is the best example of this monetization approach in action, with two distinct ways of quantifying the business of APIs.

- **AWS Marketplace Metering Service** - SaaS style billing model which provides a consumption monetization model in which customers are charged only for the number of resources they use–the best known cloud model.
- **AWS Contract Service** - Billing customers in advance for the use of software, providing an entitlement monetization model in which customers pay in advance for a certain amount of usage, which could be used to deliver certain amount of storage per month for a year, or a certain amount of end-user licenses for some amount of time.

This provides a framework for thinking about how the business of microservices can be delivered. Within these buckets, AWS provides a handful of common dimensions for thinking through the nuts and bolts of these approaches, quantifying how APIs can be monetized, in nine distinct areas:

- **Users** – One AWS customer can represent an organization with many internal users. Your SaaS application can meter for the number of users signed in or provisioned at a given hour. This category is appropriate for software in which a customer’s users connect to the software directly (for example, with customer-relationship management or business intelligence reporting).
- **Hosts** – Any server, node, instance, endpoint, or other part of a computing system. This category is appropriate for software that monitors or scans many customer-owned instances (for example, with performance or security monitoring). Your application can meter for the number of hosts scanned or provisioned in a given hour.
- **Data** – Storage or information, measured in MB, GB, or TB. This category is appropriate for software that manages stored data or processes data in batches. Your application can meter for the amount of data processed in a given hour or how much data is stored in a given hour.
- **Bandwidth** – Your application can bill customers for an allocation of bandwidth that your application provides, measured in Mbps or Gbps. This category is appropriate for content distribution or network interfaces. Your application can meter for the amount of bandwidth provisioned for a given hour or the highest amount of bandwidth consumed in a given hour.
- **Request** – Your application can bill customers for the number of requests they make. This category is appropriate for query-based or API-based solutions. Your application can meter for the number of requests made in a given hour.
- **Tiers** – Your application can bill customers for a bundle of features or for providing a suite of dimensions below a certain threshold. This is sometimes referred to as a feature pack. For example, you can bundle multiple features into a single tier of service, such as up to 30 days of data retention, 100 GB of storage, and 50 users. Any usage below this threshold is assigned a lower price as the standard tier. Any usage above this threshold is charged a higher price as the professional tier. Tier is always represented as an amount of time within the tier. This category is appropriate for products with multiple dimensions or support components. Your application should meter for the current quantity of usage in the given tier. This could be a single metering record (1) for the currently selected tier or feature pack.
- **Units** – Whereas each of the above is designed to be specific, the dimension of Unit is intended to be generic to permit greater flexibility in how you price your software. For example, an IoT product which integrates with device sensors can interpret dimension “Units” as “sensors”. Your application can also use units to make multiple dimensions available in a single product. For example, you could price by data and by hosts using Units as your dimension. With dimensions, any software product priced through the use of the Metering Service must specify either a single dimension or define up to eight dimensions, each with their own price.

These dimensions reflect the majority of API services being sold out there today, we don’t find ourselves in a rut with measuring value, like just paying per API call. Allowing government API plans to possess one or more dimensions, beyond any single use case.

- **Single Dimension** - This is the simplest pricing option. Customers pay a single price per resource unit per hour, regardless of size or volume (for example, $0.014 per user per hour, or $0.070 per host per hour).
- **Multiple Dimensions** – Use this pricing option for resources that vary by size or capacity. For example, for host monitoring, a different price could be set depending on the size of the host. Or, for user-based pricing, a different price could be set based on the type of user (admin, power user, and read-only user). Your service can be priced on up to eight dimensions. If you are using tier-based pricing, you should use one dimension for each tier.

This provides a business framework that government can provide for vendors and 3rd party developers, allowing them to operate their services within a variety of business models. Derived from many of the hard costs they face, and providing additional volume based revenue, based upon how may API calls of any particular service receives.

Beyond this basic monetization framework, I’d also recommend adding in an incentive framework that would dovetail with the business models proposed, but then provide different pricing levels depending on how well the services perform, and deliver on the agreed upon API contract. There are a handful of bullets I’d consider here.

- **Design** - How well does a service meet API design guidelines set forth in governance guidance.
- **Monitoring** - Has a service consistently met its monitoring goals, delivering against an agreed upon service level agreement (SLA).
- **Testing** - Beyond monitoring, are APIs meeting granular interface testing, along a regular testing & monitoring schedule.
- **Communication** - Are service owners meeting expectations around communication around a service operations.
- **Support** - Does a service meet required support metrics, making sure it is responsive and helpful.
- **Ratings** - Provide a basic set of metrics, with accompanying ratings for each service.
- **Certification** - Allowing service providers to get certified, receiving better access, revenue, and priority.

All of the incentive framework is defined and enforced via the API governance strategy for the platform. Making sure all microservices, and their owners meet a base set of expectations. When you take the results and apply weekly, monthly, and quarterly against the business framework, you can quickly begin to see some different pricing levels, and revenue opportunities around all microservices emerge. You deliver consistent, reliable, highly ranked microservices, you get paid higher percentages, enjoy greater access to resources, and prioritization in different ways via the platform–if you don’t, you get paid less, and operate fewer services.

This model is already visible on the AWS platform. All the pieces are there to make it happen for any platform, operating on top of the AWS platform. The marketplace, billing, and AWS API Gateway connection to API plans exists. When you combine the authentication and service composition available at the AWS API Gateway layer, with the IAM policy solutions available via AWS, an enterprise grade solution for delivering this model securely at scale, comes into focus.

**Incentivizing Government API Vendors and Contractors**
Keep everything small, and well defined. Measure, reported upon, and priced using the cloud model, connecting to a clear set of API governance guidance and expectations. The following areas can support paying and incentivizing contractors based upon not just usage, but also meeting the API contract.

- **Management** - API management puts all microservices into plans, then log, meter, and track on value exchanged at this level.
- **Marketplace** - Turning the platform into a marketplace that can be occupied by a variety of internal, pattern, vendor, 3rd party, and public actors.
- **Monetization** - Granular understanding of all the resources it takes to deliver each individual service, and understand the costs associated with operating at scale.
- **Plans** - A wealth of API plans in place at the API gateway level, something that is tied to IAM policies, and in alignment with API governance expectations.
- **Governance** - Providing a map, and supporting guidance around government platform API governance. Understanding, measuring, and enforcing consistency across the API lifecycle–platform wide.
- **Value Exchange** - Using the cloud model, which is essentially the original API management, marketplace, and economy model. Not just measuring consumption, but used to maximize and generate revenue from the value exchanged across the platform.

When you operate APIs on AWS and Azure, the platform as a service layer can utilize and benefit from the underlying infrastructure as a service monetization framework. Meaning, you can use AWS’s business model for managing the measuring, paying, and incentivizing of microservice operators. All the gears are there, they just need to be set in motion to support the management of a government API marketplace platform.

I have been studying Amazon full time for almost eight years. I’ve been watching Azure play catch up for the last three years. I run my infrastructure, and a handful of clients on AWS. I understand the API landscape of both providers, and how they can be woven into this vision for the business of government APIs. I see the AWS API stack, and the Azure API stack, as a starter set of services that can be built upon to deliver a government microservices platform. All the components are there. It just need the first set of services to be defined, delivering the essential building blocks any platform needs--things like compute, storage, dns, messaging, etc. The progress to other more outward, application, and system integration services.

My objective with this approach is to enable government services to be delivered as individual, self-contained units, that can be used as part of a larger orchestration of government services. Open up government and letting some sunlight in. Think about what Amazon has been able to achieve by delivering its own internal operations as services, and remaking not just retail, but also touching almost every other industry with Amazon Web Services. The Amazon Web Services myth story provides a powerful and compelling narrative for any company, organizations, institution, or government agency to emulate.

My proposal is not meant to be a utopian vision for how government works. However it is meant to shine a light on existing ways of delivering services via the cloud, with APIs at the center. Helping guide each service in its own individual journey, while also serving the overall mission of the platform–to help the veteran be successful in their own personal journey.
