# Testing

-  they don't add new features
- tests help with change blindness as the application gets larger. 
- tests only catch bugs when
A) you run the tests
B) the test will catch your bug
- tests need to be fast, reliable
- tests need to be modular and direct. Small enough so each function can be tested that it does it's one thing.
- broad tests are not helpful. test individual functions so you can hone in on what's causing the errors. 

## Formal Verification
- no software is inherently correct. 
- you know when software is correct when it satisfies it's list of things it should do. 

## Testing approaches
- How do I know this works or How can I break this. 
- Approaching from each of the two perspectives, misses out on a bit. 
- 100% coverage will not necessarily work to catch every error. 
- integration tests are hard
- User-Centric testing 
- Visual regression testing: more pro-active, things stay stable as you add other features
- mimic different states of your application. 
- testing environment, structures, assertion, mocks spies stubs, browser
- generate, display and watch test results
- compare and check assertions
- "Golden images" - mock ups, or stable state images. 
- use an image diffing library to compare full screen snapshots

## Headless browsers
- Makes interacting with environments easier
- Puppeteer is a library for interacting with headless Chrome that's very useful. 
- Resemble.js - visual image comparrisons
- Jest and Enzyme for React application

## example
- create directories for golden screenshots and active screenshots as well as image diffs
- golden dir, screenshot dir, diffs dir, 
- not necessarily pixel perfect, but in the ball park. 
- fresh browser via puppeteer
- navigate via route to take screenshot. 
- compare images via resembleJS - gives you percentages and other statistics
- resemble JS lays each image overtop of each other for the diffed image. 

## What to expect
- start with user stories 
- find critical points for users
- test important business logic
- maybe start with authentication
- generate a sitemap and write user stories

# CI pipeline
- guarantee a broken build is never pushed out. 