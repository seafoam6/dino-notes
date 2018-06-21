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