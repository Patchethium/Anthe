# Anthe

Anthe is an out-of-box TTS software focuses on end user experience, featured with completly offline processing, tunable voice synthesis and characterized voice banks.  

This repository maintains its GUI, which is buit with [tauri](https://github.com/tauri-apps/tauri), [svelte](https://github.com/sveltejs/svelte) and [vite](https://github.com/vitejs/vite).  

If you're looking for where the voice synthesis actually happens, check out [Anthe-training](https://github.com/Patchethium/Anthe-training).  

This project is still in its **very** early stage so don't expect you'd find anything useful here for now.  

## Development

### Fork this repository

You may find the fork button on the top right corner.

### Clone your own fork
```sh
git clone https://github.com/${your_username}/Anthe.git

cd Anthe
```
### Install dependencies

I use pnpm, but npm and yarn also works

```sh
# pnpm
pnpm install
# npm
npm install
# yarn
yarn add
```
### Launch

```sh
# pnpm
pnpm tauri dev
# npm
npm run tauri dev
# yarn
yarn tauri dev
```

### Build
```sh
# pnpm
pnpm tauri build
# npm
npm run tauri build
# yarn
yarn tauri build
```

Note: Don't create pull request on your `main` or `master` branch, create another branch like `feature/buttons` and commit there.  

Note: If your rust-analyzer reports an error in `src-tauri/src/main.rs`
```Rust
  tauri::Builder::default()
    .run(tauri::generate_context!()) // error: ... "../dist" doesn't exist ...
    .expect("error while running tauri application");
```

create a directory `dist` at the project root or build the project once and it'll disappear.

## Licence

This repository (GUI of Anthe) is released under GNU General Public License Version 3.  

## About the name

Anthe<sup>[\[wikipedia\]](https://en.wikipedia.org/wiki/Anthe_(moon))</sup>(/ˈænθiː/;アンテ) is the name of Saturn XLIX, a very small natural satellite of Saturn, named after one of the Alkyonides; the name means flowery.  

## Q&A

> So, now we don't use a UI framework?

Yes, the community of Svelte is still young, I rather style every component in tailwind css.  
