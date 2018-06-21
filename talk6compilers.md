# what is a compiler

- a code translator
- a simple JS function will be parsed/compiled into byte code
- we've been using compilers since 2013: Crockford's ...
- YUI compressor removes white space and symbol mangles
- mangling maps user assigned variables and rewrites the identifiers as a, b, c, d, etc. Big gain of 2013

## 2003 - 2008
- ES4 that never shipped

## 2008 - 2010
- the enlightenment... lots of new compilers
- cappucino, GWT, and coffeescript: tired of not having language features, they created languages that compiled to JS. 
- JavaScript is essentialy a bytecode language. 
- more advanced minifiers. Closure compiler will ignore unused code, and writes more optimal code at runtime. It's an "optimizing compiler"

## Today
- webpack, rollup, babel
- Sophisticated systems, but they do essentially the same thing as before. 
- we're expecting JS to do everything
- parse and compile is pretty expensive. 
- bytes of JS are not the same as bytes of JPGs, because the browser needs to parse and compile the JS, then execute it. Where as the JPG is decoded and painted. 

## Glimmer
- GlimmerVM: the rendering engine/virtual machine inside of ember. 
- templates are being used in Ember, 
- Angular and Vue are similar: compile the templates into javascript
- Glimmer/Ember compiles it, however, into binary so it can be read as a typed array... a slab of memory. So the code is never parsed or compiled, its read as raw memory by the JS engine.
- all of the template code no longer needs to be parsed, compiled.
- Glimmer stuff is quite a bit faster in contrived examples
- Glimmer slightly faster than preact `bit.ly/li-app`
- Glimmer uses the OpCode compiler : opcode is the operation, takes a certain amount of operands (in glimmer it can take 3)
- Glimmer templates are pushed into an operandPool. 
- the virtual machine buffs the binary and processes it. 
- things are popped out of the stack, processed, pushed back in.
- element stack flushed. 

## Web assembly
- closely aligned with glimmerVM and where the web is headed. 
- DSLs that we already have, we can convert into web assembly
- Glimmer team worked with mozilla to optimize for WASM. 
- Glimmer was rewritten in Rust to take over registers, opcodes, constants and other low level stuff.
- bit.ly/wasm-app you can see live webassembly code and play wiht it. 

- with more sophisticated compilers, we don't have to use JS for everything


