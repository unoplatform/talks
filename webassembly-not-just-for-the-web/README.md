## abstract

Most people think WebAssembly is only for the Web. Yes, WebAssembly has huge implications for the web, but also to your career as developer — it provides a way to run code written in multiple languages on the web, as client-side and server-side applications at near native speed. 

Not many people know, yet, that you can use WebAssembly to unify programming languages. Thanks to some recent advancements in the .NET community it's now possible to take existing software, compile it to WebAssembly and convert it into a .NET assembly that runs under .NET Core. 

In this session REDACTED will share with you everything you need to know and, for your viewing pleasure, port SQLite (C9X) 

to WebAssembly and concert it into a .NET assembly that is fully interoperable with "regular" SQLite builds that can read and write SQLite database files. No existing knowledge of WebAssembly or .NET is required.

## talk structure

### pre-talk entertainment

- https://binji.github.io/raw-wasm/maze/
- https://bellard.org/jslinux/vm.html?url=https://bellard.org/jslinux/win2k.cfg&mem=192&graphic=1&w=1024&h=768

### introductions

- https://platform.uno/

Display network tab during demos, you'll will see mono.wasm, this is the runtime, and it is the only wasm file, and you’ll see a bunch of .clr files, those are in fact .dlls but it’s just a hack because some entreprise firewalls block .dll files. It is automated behind the scenes by the uno.wasm.bootstrap package.

- https://playground.platform.uno

 

- https://calculator.platform.uno/

### what is webassembly

- https://webassembly.studio/
    - wasm vs wat
    - hello world
    - Show output .wasm file
    - Create Add Method and show output again (see the method was optimized)

- https://hacks.mozilla.org/2018/10/webassemblys-post-mvp-future/


#### wasi

- https://wasi.dev/

#### exciting developments

- https://medium.com/wasmer/webassembly-sh-408b010c14db

CDNs are positioned to eat cloud providers - "Do we really need docker?"

- https://www.fastly.com/blog/announcing-lucet-fastly-native-webassembly-compiler-runtime

### dotnet

#### mono

- Uno runs on Mono
- Blazor runs on Mono

Let's show you how it works:

- New .netstandard 2.0 class library
- Install Uno.wasm.bootstrap from nuget
- Demo console writeline  (show that it’s visible in the browser console)
- Demo invokeJS    (requires the binding.cs file included in sample code)  Shows that it’s possible (but tedious) to modify the DOM.
 
Preparation
- Steps to prepare are here : https://github.com/nventive/Uno.Wasm.Bootstrap
- To deploy the dist to localhost, use Ubuntu on Linux subsystem : https://github.com/nventive/Uno.Wasm.Bootstrap#server-the-wasm-app-through-windows-linux-subsystem

#### wasm2cil

- https://github.com/ericsink/wasm2cil
- https://ericsink.com/entries/wasm_wasi_dotnet.html

### 


