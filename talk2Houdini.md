# How you can write a rendering engine

  - API to extend browsers. 
  - To add a new property: have an idea -> Specification (algorithm, ) -> different browsers implement it differently -> it works?
  - Not everyone can take part in it, since you need to go to conferences, and attend
  - Houdini takes away the need to have it in committee as well
  - the browsers might not invest money into implementation. Every added feature is more tech debt. 
  - FREDs have to deal with the technical debt for end users. 

## Solution?

- Using the extensible web manifesto. Browser rendering engines make low level APIs for developers
- these APIs are standardized and let the vendors work on optimizing low level code. 
- Houdini lets developers innovate and build the stuff before taking it to committee. 

## APIs

- Worklets: light weight interfaces like webworkers that have very specific use cases. 
- add module pointing to your worklet file
- custom paint API lets you generate an image
- register the file, then have a callback. 
- BENEFITS: reduced dom, reduced code

## CODE
- bit.ly/rawr-properties

## Properties and Values

- register properties and make sure they fit the standard for valid CSS properties ( color in this example)

## Typed OM
- css object module
- a cleaner way to write properties without strings
- the browser forces everything as a string when it returns it to you
- in typed OM though, you actually use the correct type (numbers, etc)
- better performance, better error handling

## Animation worklet
- add a module, reference a worklet file
- target a dom element, make keyframes
- register a class, make a callback, animate function, constructor for defaults
- Benefits: Performant

## Custom Layout Worklet
- similar set up to the other worklets
- Layout (children, constraintSpace, styleMap)
- lots of performance gains, you can ignore layout modules you're not going to be used

## Can I Use?
- iswhodinireadyyet.com
- mostly on chrome
- bit.ly/houdini-dinosaur
