# Web assembly

Jay Phelps @_jayphelps

- WASM: byte code for the web
- efficient: fast to load and execute. 
- Streaming compilation: compiled faster than it downloads.
- JavaScript parsing and compiling is pretty slow. 
- compiled to machine code
- web assembly is intended to be a compilation target: Written in C or Rust.
- WASM is safe and portable: buffer overrun and other exploits are not possible.
- Wasm is like a shortcut to your javaScript engine's optimizer. 
- Why not compile JS to WASM? One day maybe it will replace JS with other compiled languages ELM/Reason
- JavaScript is extremely dynamic. Compiling JS to web assembly would be slower
- v1 is better suited for C/C++/Rust
- Java and OCaml are the next targets
- TurboScript is a language designed around WASM
- WASM uses the typescript parser, and looks the same as TypeScript
- WASM oxidizes source maps in Firefox, Babel, Less. Parsing is 10.9x faster
- Sass uses C++, and takes forever to install because you need to compile it. Currently there's an effort to port it to webassembly.
- d3-wasm-force big improvement on d3

- binary is intimidating 
- don't worry about the binary. Let the tooling take care of it. 
- textual representations abstract away the need to worry about binary

- WASM is a stack machine language. It pushes and pops on a stack machine. These are the only 2 operations available. 
- Last in First Out 

- compilers do exotic optimization for you. 
- most tooling supports Abstract Syntax Tree (AST)
- AST is still compiled and evaluated as a stack machine
- AST uses s-expressions that were invented by Lisp

## What's missing

- direct access to the dom is not there. 
- any time something is going to be displayed, it has to be called into javascript
- the spec is being worked on now
- garbage collection: the JS garbage collection doesn't see WASM and ignores it. You need to import in your own garbage collector, currently.
- multi-threading: True multi-threading is complex. Introduces a lot of race conditions. 
- the spec is advancing quickly. Microsoft, apple, mozilla all on the same page to unify the spec. 
- Reason React could run web assembly
- checkout awesome-wasm repo
- all modern browsers support web assembly. 

- web assembly is going to revolutionize how code is written and consumed.
 
