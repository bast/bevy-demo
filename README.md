# [Bevy](https://bevyengine.org/) game example deployed via GitHub Pages

This demo shows how to deploy a [Bevy](https://bevyengine.org/) game to GitHub
Pages using WASM.


## Code and knowledge copied from other places

- Breakout example and assets copied from https://github.com/bevyengine/bevy
  (MIT license).
- I experienced a problem with sound and found a solution in https://deepstacker.com/2021-07-08-bevy-in-the-browser/.
- The solution is copied from https://developer.chrome.com/blog/web-audio-autoplay/#moving-forward (CC-BY-SA-4.0 license).


## Local preview in the browser

Preview with:
```
$ trunk serve
```

Prerequisites:
```
$ cargo install trunk
$ rustup target add wasm32-unknown-unknown
```


## Native build on NixOS

```
$ nix-shell
$ cargo run [--release]
```
