# Visualisation Webgpu Tooling Project

I am helping out with the [rtvis-webgpu-tutorial](https://github.com/Welko/rtvis-webgpu-tutorial) for the 193.166 Visualisierung VU. This is the project documentation for it.

## Tutorial

Link: https://github.com/Welko/rtvis-webgpu-tutorial

**Tasks**

The tutorial improvement tasks are not yet fixed, am still coordinating with Patrick. 

- [x] Helping out with updating the tutorial for WS25 https://github.com/Welko/rtvis-webgpu-tutorial/pull/1
- [ ] Updating the tutorial project tooling for WS26 https://github.com/Welko/rtvis-webgpu-tutorial/pull/13
  - Problem: We want language server support. This requires having the WGSL shader code in separate `.wgsl` files.\
    However, loading such files from disk requires a local web server.
  - Solution: Adopt the industry standard [vite](https://vite.dev/) tool as the local web server.\
    This also lets us directly load the dataset from disk, instead of having to jump through hoops. It's a big upgrade.
- [ ] Switch from Node.js to Deno
- [ ] Switch from Node.js to using a VS Code live server extension
- [ ] Add online playground for the tutorial.
  - Problem: The new tooling depends on having Node.js/Deno installed.
  - Solution: Having an online version of the tutorial, [hosted on Stackblitz](https://stackblitz.com/~/github.com/Welko/rtvis-webgpu-tutorial), solves this. 
- [ ] Improve shader compilation error messages
  - Not yet started
- [ ] Automatically suggest installing wgsl-analyzer when opening the tutorial project
- [ ] Stretch goal: Running wgsl-analyzer in the web

**Documentation**

TODO

## Tutorial Slides

**Tasks**

- [ ] Extend the slides with WebGPU fundamentals

## Language Server

Link: https://github.com/wgsl-analyzer/wgsl-analyzer

**Tasks**

- [x] Ship stable version of wgsl-analyzer https://github.com/wgsl-analyzer/wgsl-analyzer/releases/tag/2025-11-14
- [x] Manually test with tutorial code
- [ ] Automated tests for features used in tutorial code
- [ ] Top tier support for more IDEs
  - [ ] Neovim
  - [ ] Stretch goal: Visual Studio for the teams that use WebGPU with C++

**Documentation**

[Installing the language server](https://wgsl-analyzer.github.io/book/installation.html) is usually done by [installing it from the Visual Studio Code marketplace](https://marketplace.visualstudio.com/items?itemName=wgsl-analyzer.wgsl-analyzer).

More documentation will come, as more tasks are completed

