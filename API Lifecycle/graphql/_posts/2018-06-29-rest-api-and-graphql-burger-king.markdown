---
published: true
layout: post
title: GraphQL And REST Differences Explained With Burgers
date: 2018-06-29T09:00:00.000Z
tags:
  - API Evangelist
  - GraphQL
  - Politics of APIs
image: 'https://s3.amazonaws.com/kinlane-productions/graphql/graphql-book.png'
---
GraphQL folks keep on with the GraphQL vs REST narratives, rather than a REST and / or GraphQL narrative lately with [a recent burger meme/narrative](https://twitter.com/NikkitaFTW/status/1011928066816462848). Continuing to demonstrate their narrow view of the landscape, and revealing the short lived power of an adversarial approach to community building. I get why people do this, because they feel they are being clever, and that the click response from the echo chamber re-enforces it, but ultimately it is something that won't move the conversation forward, but it does get them kudos within their community--which is what many of them live for.

<p align="center"><img src="https://s3.amazonaws.com/kinlane-productions/graphql/graphql-book.png" align="center" width="75%"></p>

I'll start with the usual disclaimer. I actually like GraphQL, and prescribe it as part of my API toolbox. However, rather than a REST vs GraphQL approach, I sell it as REST and GraphQL, depending on the developer audience we are trying to reach with our efforts. Whether or not you use GraphQL on your platform is completely based upon knowing your developers, and working with a group that understands the resources before offered--something the GraphQL community continues their failure to see. Also their adversarial marketing tactics has lost me several GraphQL projects in government because it comes off as being a trend, and not something that will be around very long.

With that said, I think this meme tells a great story about GraphQL, and demonstrates the illnesses of not the technology, but the ideology and beliefs of the community. I had a couple of thoughts after seeing the Tweet, and reviewing the replies:

1) I thought it was an anti-GraphQL meme at first. Demonstrating that you can build a horrible burger with some very well known ingredients. [Spoofing on the burger emoji drama that has been going on in recent years.](https://www.theverge.com/2017/10/30/16569346/burgergate-emoji-google-apple). I mean, is the lettuce the plate in the GraphQL burger?

2) Like GraphQL, the food choices demonstrate that GraphQL works well in very controlled environments. Where there are known ingredients, and your clients/customers/developers know the ingredients, and know what they want. Hell yeah GraphQL is a better choice in this environment. The problem is you are selling it as a a better solution than REST in general. I hate to tell you, but most of the business getting done in the world IS NOT FAST FOOD.

3) The meme demonstrates the whole fast food, limited world view of many technologists who work with known ingredients, and think everyone is just like them. This tool works for me, and everyone is just like me, so what I use is cool, and everyone should use the tools and the process that I do. A common perspective out of the white bread (bun?) world of technology.

4) Let's take this GraphQL meme and begin applying it to an Ethiopian, Greek, or French menu. Let's take it and apply to a BBQ, catering, or maybe home cooked family gathering. Try applying it when you get a food basket from your local community supported agriculture (CSA), where you have no idea the ingredients that are coming, and you'll have to adjust based upon the season and whatever is available to you that week. Maybe do the same for a food shelter and pantry, does everyone get it their way?

5) There are some restaurants in New York I'd love to take you to, and have you ask for it your way. I'd love to see you get yelled out of the place when you think you know more than the chef, and you always should have things your way. Really, you know more than someone who has been cooking for years, and your fast food loving, unsophisticated tastes are going to dictate what gets served? Get outta here!!

6) I love API to restaurant menu analogies. I wrote one [to support the Oracle v Google copyright case](https://apievangelist.com/2014/05/23/restaurant-menus-as-analogy-for-api-copyright/), which [the Google lawyer referenced in the latest round](https://apievangelist.com/2014/05/23/restaurant-menus-as-analogy-for-api-copyright/). There are many ways you can use restaurants and food to make API comparisons, and educate people about the potential of APIs. I'm sorry though, this one just wasn't sophisticated enough to really bring home the potential of APIs, and it was more about reflecting this same unsophisticated approach of people marketing and telling stories around GraphQL.

I'll say it again, and again, and again. I'm not anti-GraphQL. I'm against ya'll saying it is a replacement for REST. Stop it. It's dumb. It shows your lack of awareness of the larger API world. It shows you live in tech isolation, where you think everyone wants it your way. Most developers I know do not have a clue as to what they want. They don't understand the existing schema being used, and need menus, and hand-crafted buffets. Sure, there are development groups who know exactly what they need, and have a full grasp on the schema and resource models being used, but this isn't EVERYONE!! Stop it. I get GraphQL, but I'm getting tired of coming across new APIs I don't understand at all, and being expected to just know what I want. I love GraphQL for Github because I KNOW GITHUB. I don't love GraphQL for [the OpenStates API](http://docs.openstates.org/en/latest/api/v2/), because I have no clue what the schema and model is for their API--please do the extra work to document your resources, and provide me intelligent, well-crafted paths to get at your valuable data.

Instead of bashing REST, how about thinking more about REST as a starter. Having feedback loops in place to get to your audience. Sure, if it is all internal development, in service of a known group of React developers, go for it--use GraphQL! However, if it is a public API, start with REST, establish feedback loops, and get to know your audience. If enough developers are requesting a query language (GraphQL isn't the only show in town), and it makes sense in your roadmap, then offer GraphQL alongside REST, but not instead of REST. GraphQL works in a known known, and sometimes a known unknown environment, but not in an unknown unknown environment. The community needs to wake up and realize this. Stop selling it as a replacement to REST, and realize it is just another tool in the API toolbox. Y'all are just hurting your cause, and running some people off with this regular REST v GraphQL storytelling. In the end, you are just showing your lack of knowledge and respect for the web--just like Facebook does.

P.S. Anyone who has their feelings hurt by this post, needs to get out more. Maybe change jobs, move to a new city and industry. You need to see and experience more than you have currently.
