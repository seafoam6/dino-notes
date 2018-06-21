Jennifer Wong

# Empathetic Design Systems

- design systems are trendy. 
- 2013: Atomic design coined
- A complete set of deign standards with principles and a tool kit
- pattern library, component library, style guide ... these are all types of design systems. 

## Examples

- spectrum by adobe: private, a larges system
- US Web Design System: 18F open source made by the gov: Used by gov agencies
- Mozilla has a styleguide that hasn't been updated in years. 
- Mozilla has a photon design system as well

## Empathy

- The ability to share feelings with another
- "in feeling"

## UX PIN

- most problems facing design teams can be boiled down to empathy issues. 
- Frontend foundry team: 3 seniors, 3 entry level

## StyleGuide

- KSS - last updated 2 years ago
- brittle, no way to add new systems
- cascade overwrote things
- lots of finagling things to get them to work

## Eventbrite Design System
- design systems are living funded product with a roadmap, backlog
- component generator using plop.js
- command line tool to add new components
- planned approach for adding a component, discuss edge cases, props with design and devs
- accessability with eslint-accessability
- design system has problems from lack of empathy.
- when you come to a design system, you search from them... and if you don't know the name. 
- dropdown is a subcomponent of dropdown... naming things is difficult. 
- it was difficult to tell if a component is deprecated. What does "unstable" "subject to change" mean? How does one get more information?
- design team delayed by dev building new component.
- it's difficult to tell which component you should use in a given scenario, especially when components have similar abilities
- The code is not accessable by design team
- differences between grid systems and alignment
- release process was complicated

## solutions backed by empathy
- created a better search, make things more discoverable. 
- less spacing, so you could see more
- small screenshots of each of the components so you could see them at a glance
- stopped using acronyms. Purged code base of it. 
- weekly meetings and a slack channel
- component usage guidelines, so you know when to use a component
- use react studio for prototyping with the designer
- started bumping twice a week to better coordinate releases

## Empathize
- who will use it?
- think of all the ways a person will use a design system. 
- tell everyone about the system, so knowledge is shared
- write documentation
- have a centralized place

## help with design systems
- storybook
- UX Pin: UX design platform