# Critical Request

- performance of users: various places, various connection speeds
- User loses focus after 1 second
- abandon after 10 seconds

# steps

- user navigates
- first paint
- first contentful paint
- first meaningful paint (content above the fold)

- load and render time line. onLoad isn't useful. 
- first meaningful paint is. Text and lead content is painted.

- critical request is essential to the content in the viewport
- css, fonts, logo, lead image

# resource queuing

- stuff in the head tag
- in devtools, turn on priority in the network tab. 
- As the browser reads the file, it assigns priority to each resource
- html - highest
- css - highest
- images - low or medium priority (in Chrome, above fold is bumped to medium priority)
- xhr high
- fonts - highest
- scripts - low/med/high. Placed before img, scripts are high or medium. async/defer are low.

# fonts
- stylesheets
- looks for font face
- finds text to render
- not having text, delays the paint. 

# auditing 

- Atlassian 
- audit: Turn on screenshots. Set to fast 3g, 4x slowdown on cpu. 
- disable cache
- record, reload page. 
- purple are paints
- yellow is scripts
- red JS thread is receiving a bunch of stuff, being blocked

- text not readable because the webfonts are loaded as the 30th request
- add crossorigin tag is necessary for fonts `<link rel="preload" href="font.woff" as="font" crossorigin>`
- OR you can set this as a HTTP header
- enable local overwrites, this lets you overwrite stuff locally.
- preload all the fonts.
- trims 4-5 seconds off of render
- font-display: swap; css property: this allows you to display standard font until webfont is available, then swap them. 
- meowni.ca/font-style-matcher lets you compare fonts rendered over each other, so the size doesn't jump. 
- use woff2 where available

- priority hints is in proposal, and hidden behind a chrome flag. 

# Checklist
- audit in poor conditions
- use the performance panel to explore relationship between render, assets, fetching, paints and execution
- ensure critical requests are given priority
- become a performance advocate
- bake performance into all parts of the project timeline

- make a performance workbook: Estimated gain / achieved gain / difficulty / estimated cost
- test everything: come up with numbers
- automate testing
- draw conclusions from actual data



