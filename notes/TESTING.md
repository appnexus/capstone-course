# Testing Thinking

## What is Testing?
* Process of evaluating a system or its components with the intent to find whether it satisfies the specified requirements or not
* In simpler terms: Checking if something acts the way that it should

## Why Test? (part 1)
* No one writes perfect code
* Even when your code performs correctly in isolation, it may not function as intended with code that others (or past you) have written
* Benefits:
  * Catch more bugs, catch bugs earlier, prevent bugs from reaching users
  * Appropriate confidence (hopefully more!) in writing, merging, and deploying code
  * Improved software design and architecture
  
## How does one test?

### Anatomy of a Test Case
* Steps
  * Given - setup for the test case
  * When - action taken to exercise whatever you are testing
  * Then - assertion that checks if actual behavior matches expected behavior
* Result
  * Pass - all assertions are run, and actual behavior matches expected behavior
  * Fail - at least one assertion resulted in actual behavior NOT matching expected behavior
  * Error - an unexpected problem occurred before the test could finish
* Example: Testing iPhone X for Waterproof-ness
  * Given an iPhone X and a pool of water 1m deep
  * When I submerge the iPhone X in the pool, and wait for 30 seconds, and retrieve the iPhone X
  * Then I am able to make a phone call, and play music through the speakers, and send a text message with no change in quality

### Manual vs Automated Testing
* Manual Testing
  * Pros: no overhead of learning how to use testing frameworks
  * Cons: becomes tedious and time consuming, does not scale well
* Automated Testing
  * Pros: machines are good at doing lots of tedious and time consuming things, much more likely to scale well
  * Cons: need to learn how to use testing frameworks and tools, and actually write the tests

### Spectrum of Automated Testing


## Links to resources

### [Google SRE Chapter 17 (Testing)](https://landing.google.com/sre/book/chapters/testing-reliability.html)

### [Tutorials Point Software Testing Intro](https://www.tutorialspoint.com/software_testing/)
