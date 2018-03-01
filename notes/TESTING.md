# Testing Thinking

## What is Testing?
* Process of evaluating a system or its components with the intent to find whether it satisfies the specified requirements or not
* In simpler terms: Checking if something acts the way that it should

## Why test? (part 1)
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
|Type of Testing|System Under Test|Common Tools|Example Test Case|
|---|---|---|---|
|Unit Tests|Function or Class|xUnit|Given the list [1, 0, -1]<br><br>When I run the sort() function<br><br>Then the output should be [-1, 0, 1]|
|Integration Tests|An "Assembled Component" (e.g. single application or program)|xUnit, Selenium|Given the Huntergram API and a mock DB of users and passwords (including `user123` and `pass123`)<br><br>When I HTTP POST to /auth service with `{"username":"user123", "password":"pass123"}`<br><br>Then I should receive a `200 OK` and my session token in `Set-Cookie`|
|System Tests|Multiple applications working together|Selenium|Given the Huntergram API and a mock DB of users and passwords (including `user123` and `pass123`)<br><br>When I enter `user123` as username and `pass123` as password and click `login`<br><br>Then I should see my home page|

### Concepts to Keep in Mind
* Minimize dependencies for whatever you are testing
  * If you only need to implement 2 classes rather than 20 in order to use a given function, then:
    * You can start testing much earlier (don't need to finish as many classes before testing)
    * Your test will likely better reflect production functionality (since you don't have to have as many mocks)
    * Your codebase is more resilient (changing other parts of the codebase are less likely to affect this function)
* Diminishing returns of testing
  * The first test and the first several tests you write are incredibly valuable
  * Very complex or unlikely setups yield much less value per test case, and may not be worth writing (depending on your context)
    * Are you working independently on a small script? Maybe just one test case
    * Are you working on a team for a low-risk school assignment? Maybe several, common test cases
    * Are you working for NASA on a billion dollar project? Test ALL the things
 * Regression testing - "Fool me once, shame on you; fool me twice, shame on me"
   * Whenever you finish debugging a bug, immediately write and add a test that would catch it.
   * Whenever you make a change to your code, run all the tests that have been written thus far. You (and your whole team) should never hit the same bug again!

## When does on test? Why test? (part 2)
* Before and During Development (Test Driven Development, a.k.a. TDD)
  * ex: When writing a new class, define all your functions first and have them return a valid default / dummy response. Then write out all of your test cases. Once finished, your tests should all run and all fail. Then, as you actually develop your code, the tests should slowly start to pass. If you have written your tests in alignment with your story's Acceptance Criteria, then you should be functionally complete once all the tests pass!
  * Benefits
    * Better aligns your code with your story's ACs
    * Forces you to think of your design (e.g. what functions do I need) before starting to code
    * Provides you with clear indicators of progress as you develop
* Whenever code changes are "integrated" (Continuous Integration, a.k.a. CI)
  * ex: Whenever you want to make a commit or merge a PR, run all of the tests. This means that you should catch test breaking changes right as you make the code changes, rather than several commits or merges down the line.
  * Benefits
    * Very fast and consistent way to run tests + catch bugs
    * Easy to roll back to a known good version if something goes wrong (simply look for the last time that all the tests passed)
    * Free Github integrations with Travis CI

## My Suggestions
* As you are exploring your various technologies, find out how to unit test each of them and write at least ONE test
* Configure an automated build integration with Travis CI and your Github repo (docs below)
  * Note: this doesn't need to do anything right now beyond running a successful build
* As a team, define and agree upon at least 1 manual, system-level (end-to-end) test
  * This can be a useful baseline for when your team has all components up and running
  * Can be automated and expanded if you have time

## Links to resources

### [Google SRE Chapter 17 (Testing)](https://landing.google.com/sre/book/chapters/testing-reliability.html)

### [Tutorials Point Software Testing Intro](https://www.tutorialspoint.com/software_testing/)

### [Travis CI with Github Guide](https://docs.travis-ci.com/user/getting-started/)

### [List of Unit Testing Frameworks](https://en.wikipedia.org/wiki/List_of_unit_testing_frameworks)

### [Selenium Home Page](https://www.seleniumhq.org/)
