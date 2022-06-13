# Anthe

Anthe is an out-of-box TTS software focuses on end user experience, featured with completely offline processing, tune-able voice synthesis and characterized voice banks.  

This repository maintains its GUI, which is built with [tauri](https://github.com/tauri-apps/tauri), [svelte](https://github.com/sveltejs/svelte) and [vite](https://github.com/vitejs/vite).  

If you're looking for where the voice synthesis actually happens, check out [Anthium](https://github.com/Patchethium/Anthium).  

This project is still at its **very** early stage, don't expect you'd find anything useful here for now.  

## Development

We recommend to use [Visual Studio Code](https://code.visualstudio.com/) or its OSS alternative [VSCodium](https://vscodium.com/) for the best developing experience. Also, install the following extensions:

- Svelte for VS Code
- rust-analyzer
- PostCSS Language Support
- ESLint
- Tailwind CSS IntelliSense
- Tauri

Note: You may need to download and install some of the extensions manually if you're using VSCodium. 
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

Note: Don't commit on your `main` or `master` branch, create another branch like `feature/buttons` and commit there.  

Note: If your rust-analyzer reports an error in `src-tauri/src/main.rs`
```Rust
  tauri::Builder::default()
    .run(tauri::generate_context!()) // error: ... "../dist" doesn't exist ...
    .expect("error while running tauri application");
```

create a directory `dist` at the project root or build the project once, restart the editor and it'll disappear.

## License

This repository (GUI of Anthe) is released under Apache License, version 2.0.  

## About the name

Anthe<sup>[\[wikipedia\]](https://en.wikipedia.org/wiki/Anthe_(moon))</sup>(/ˈænθiː/;アンテ) is the name of Saturn XLIX, a very small natural satellite of Saturn, named after one of the Alkyonides; the name means flowery.  

## Q&A

> So, we don't use a UI framework?

Yes, the community of Svelte is still young, I rather style every component in tailwind css.  
