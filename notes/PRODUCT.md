# Product Thinking
The art of defining and solving a problem with a specified target audience, strategy, and goal in mind.<br>
Disclaimer: This does not cover aspects of a business idea or proposal which include market research, competitor analysis, advertising etc. <br>
The goal is to focus on shaping the thought process in defining a product keeping in mind the user, the experience, and how to come up with realistic achievable goals and features in order to achieve them.

## Defining your product
The following layout helps define your product:
In order to ______ (vision) <br>
our product will solve ______ (target audience) <br>
problem of ______ (user problem) <br>
by giving them ______ (strategy).  <br>
We know if our product works when we see a ______ (goal). <br>

This section adpated from Reference 2.
### User First
Define "who" has "what" problems?
#### Problem
What is the problem we are trying to solve
#### Audience
Whom are you going to solve the problem for (go hand in hand)

### Job to be done
Define the vision and "how" shall we do this?
#### Vision
Why are we doing this?
#### Strategy 
The how will we do this. #1 rule : Solve the problem first

### Output
Define features and how do we measure the success?
#### Goals Setting
What do we plan to achieve? What goals are we setting?
#### Features
What features will this manifest as? What will we do to reach our goals?

## Example

### User
Locals looking for things to do

### Problem
Often do I see myself looking up for things to do, sometimes I don't know what I want or what's going on around, have too many specialized apps/sources instead of a single source which be overwhelming to go through.

Lack of a unified source for local:
1. Recommendations for things to do across diverse domains
2. Unified experience across different aspects
3. Personalized to your taste

### Vision
One stop personalized recommendation engine for local events and things to do

### Strategy
How do we plan to plan, build, monetize etc. Vision and strategic thinking (UX) are a must for a successful product.
Includes the following: 
1. What form will this be available to the user? An app, personal assistant in the form of say Alexa/robot etc.
2. Sample approach: (top down): Defining Product vision, goals, defining roadmap in order.
3. How will you on board new users, how will you get the access to various data sources/feeds etc.
4. When and how will you monetize? Will the app be free at first?
The list goes on. However, this some parts of this are out of scope of this discussion.

### Goals
Coming up with product goals is the step that helps you translate your product strategy into an executable plan.
1. Personalization: A recommendation engine personalized to your hobbies, interests, recent activities, spending patterns etc.
2. Social Media: Leverage the power of social media to enhance your experience
3. Monetization: Either through ads, a revshare of the local deals, restaurant recommendations etc.
4. Secure: Means for authorization, authentication, secure access over say https etc.
5. Plan, organize my schedule: Ability to subscribe to events, plan my activies, manage my calendar, setup alerts/reminders etc.

### Features
Product features are specific means to achieving the goals you have set out. A goal usually has many features, but a feature delivery may attribute success in achieving a multiple goals. 
Here are some examples of features for say "Social Media" goal.
1. Show places recently visited, tweeted or posted by friends on social platforms like Facebook, Twitter, Instagram.
2. Ability to like/dislike a post in Facebook
3. Ability to re-tweet a post you like 
5. A timeline of events of your friends for the same
6. Ability to organize an event say dinner by inviting your social friends

## Mapping goals and features into agile methodology
Having gone through the process of product thinking, laying out our goals and features, we can map them into epics, stories and sub-tasks in agile methodoly. Here is an example for the sample use case above: 

### Epic
While this is not a hard rule, an epic in this case eg. "Leverage Social Media to enahance user experience" can roughly map to a goal.

### Stories
Each story in this case can map to a feature.
1. As a user, I would like to show places recently visited, tweeted or posted by friends on social platforms like Facebook, Twitter, Instagram <br>
2. As a user, I would like to restrict access of my recommendations, private events, and personalized experience to myself. No one else should see this. <br>
3. As a user, I would like the ability to oragnize community event(s) of a specified genre and be the administrator of the event.
...

### Sub-tasks
Lets pick social media to be the story. Following sub-tasks need to be performed under a story to achieve it.
1. Parse friends' Facebook posts leveraging API given current location, user id, and time interval
2. Parse friends' Twitter tweets leveraging API given current location and user id, and time interval
3. Parse Instagram feed leveraging API given current location and user id, and time interval
4. Store in an in memory database (say client side) optimized for fast reads
5. Refresh the feeds every 5 minutes
6. Define a unified interface for feeds retrieval
7. Design a UI page to represent the friends' activity
...

## Links to resources
1. [Product Thinking is Problem Solving](https://www.interaction-design.org/literature/article/product-thinking-is-problem-solving)
2. [Why Product Thinking is the next big thing in UX Design](https://medium.com/@jaf_designer/why-product-thinking-is-the-next-big-thing-in-ux-design-ee7de959f3fe)
