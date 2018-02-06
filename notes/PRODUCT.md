# Product Thinking
The art of defining and solving a problem with a specified target audience, strategy, and goal in mind.

_Disclaimer_: This does not cover certain aspects of a business idea or proposal which include market research, competitor analysis, advertising etc. However user research to define the problem is still relevant.

The goal is to focus on shaping the thought process in defining a product keeping in mind the user, the experience, and how to come up with realistic achievable goals and features in order to achieve them.

## Defining your product
The following layout helps define your product:
In order to ______ (vision)

our product will solve ______ (target audience)

problem of ______ (user problem)

by giving them ______ (strategy).

We know if our product works when we see a ______ (goal).


This section adpated from Reference 2.
### User vs. problem first
Define "who" has "what" problems
#### Problem
What is the problem we are trying to solve
#### Audience
Whom are you going to solve the problem for (go hand in hand)

While both user and the problem go hand in hand, there are two ways to approach them:
1. _User first:_ A lot of products go identify their target audience first and then get find real problems to solve from them. Eg. audience can be rich people or organizations if your strategy is to monetize. You are likely to find a real problem to solve from them. Eg. Appnexus has strategic partners who describe their problems and products are built to solve for them.
2. _Problem first:_ The product is built on an problem in mind, however this needs to follow up with user research in order to identify your target audience, or validate whether the problem is indeed worth pursuing. Eg. Google search.

### Job to be done
Define the vision and "how" shall we do this?
#### Vision
Why are we doing this and what an ideal world looks like?
#### Strategy 
How will we do this. #1 rule : Solve the problem first

### Output
Define features and how do we measure the success?
#### Goals Setting
What do we plan to achieve? What goals are we setting?
#### Features
What features will this manifest as? What will we do to reach our goals?

## Sample example
### Problem
Often do I see myself looking up for things to do, not knowing know what I want or what's going on around. There are many specialized apps/sources for food, events etc. instead of a single source. It takes a lot of effort to go through each one of them and plan my day or weekend.

In summary, there is a lack of a unified platform for local area recommendations that provides a unified user experience, personalized to the user's taste.

### User
Locals looking for things to do

### Vision
One stop personalized recommendation engine for local events and things to do

### Strategy
Vision and strategic thinking are a must for a successful product. Strategy defines _how_ do we plan to approach and build the solution. Includes various aspects of which the some are out of scope.
#### Within scope:
1. In what form will this be available to the user? An app, personal assistant via Alexa/robot etc.
2. Sample approach: (top down): Defining Product vision, goals, defining roadmap in order.
3. Order of deliverables: UX comes first, followed by an MVP UI mock up, with a full fledged backend and other features to follow.
#### Out of scope:
1. How will you onboard new users?
2. What business deals will you need to get access to various data sources/feeds etc.?
3. How will you monetize? Will the app be free at first?
The list goes on.

### Goals
Coming up with product goals is the step that helps you translate your product strategy into an executable plan.
1. Personalization: A recommendation engine personalized to your hobbies, interests, recent activities, spending patterns etc.
2. Social Media: Leverage the power of social media platforms like Facebook, Twitter etc. to enhance your experience by sharing friends' local activities.
3. Monetization: Either through ads, revenue sharing of the local deals, restaurant recommendations etc.
4. Security: Means for authorization, authentication, secure access over https etc.
5. Plan, organize my schedule: Ability to subscribe to events, plan my activies, manage my calendar, setup alerts/reminders etc.<br>
...

### Features
Product features are specific means of achieving the goals you have set. A goal usually has many features, but a feature delivery may attribute success in achieving a multiple goals. 
Here are some examples of features for "Social Media" goal:
1. Show places recently visited or posted by friends on social platforms like Facebook, Twitter, Instagram
2. Ability to respond eg. like/dislike a post in Facebook
3. A timeline of events of your and your friends' activity over the past 2 weeks/month/year

## MVP strategy
Now that we have defined the goals and features for our product, the efforts to build them all can be large. A minimum viable product (MVP) is a development technique in which a product is developed with sufficient features to satisfy early adopters. In this course, you shall learn the value of delivering an MVP. You can put out the product for early adopters to get feedback on the experience. Small investment, big return.
Eg. A simple app backed by a recommendation engine for various local events/things to do, user login, and a UI would serve the purpose. Advanced personalization, social feed, monetization strategies, imrpoved feeds, frequent refresh rates etc. are examples of features that can come along in a full fledged product.

## Mapping goals and features into agile methodology
Having gone through the process of product thinking, laying out our goals and features, we can map them into milestones, epics, and stories in agile methodoly. Here is an example for the sample use case above: 

### Milestone
While this is not a hard rule, a milestone in this case eg. "Leverage Social Media to enahance user experience" can roughly be mapped into a goal.

### Epic
Each epic in this case can be mapped  into a feature.
1. I would like to show places recently visited or posted by friends on the Facebook social platform
2. I would like to restrict access to my recommendations, private events, and personalized experience to myself. No one else should see this
3. I would like the ability to oragnize community event(s) of a specified genre and be the administrator of the event

### Stories
Let's pick epic #1 above as an example. The following stories need to be performed under the story to achieve it.
1. As a user, I would like to parse friends' Facebook posts leveraging API given current location, user id, and time interval so that I can retrieve friends' social activity
2. As a user, I would like to quickly retrieve friends' Facebook activity so that I can have optimial user experience. Sample engineering work for this could be to store the parsed Facebook (encrypted on the client side) optimized for fast reads.
3. As a user, I wish to refreshed friends's Facebook activity (within last x minutes) so that I am always up to date
5. As a user, I wish to see the friends' Facebook activity on a UI so that I can have a rich user experience

## Links to resources
1. [Product Thinking is Problem Solving](https://www.interaction-design.org/literature/article/product-thinking-is-problem-solving)
2. [Why Product Thinking is the next big thing in UX Design](https://medium.com/@jaf_designer/why-product-thinking-is-the-next-big-thing-in-ux-design-ee7de959f3fe)
