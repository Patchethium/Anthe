# Anthe

Anthe is an out-of-box TTS software focuses on end user experience, featured with completely offline processing, tune-able voice synthesis and characterized voice banks.

This repository maintains its GUI and inference code. If you want to train a model, check out [Anthium](https://github.com/Patchethium/Anthium).

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

## Prerequisites

The tech stack we use is Rust, 

### Clone your own fork
```sh
git clone https://github.com/${your_username}/Anthe.git

cd Anthe
```
### Install dependencies

We use [pnpm](https://pnpm.io/), node version 18.4.0.

```sh
pnpm install
```
### Launch

```sh
pnpm tauri dev
```

### Build
```sh
pnpm tauri build
```

Note: Avoid committing on the `master` branch, create another branch like `feature/buttons` and apply your change there.

Note: If your rust-analyzer reports an error in `src-tauri/src/main.rs`
```Rust
tauri::Builder::default()
  .run(tauri::generate_context!()) // error: ... "../dist" doesn't exist ...
  .expect("error while running tauri application");
```

create a directory `dist` at the project root or build the project once, then restart the editor.

## License

This repository (GUI of Anthe) is released under Apache License version 2.0.

## Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in the work by you, as defined in the Apache License version 2.0, shall be licensed as described above, without any additional terms or conditions.

## About the name

Anthe<sup>[\[wikipedia\]](https://en.wikipedia.org/wiki/Anthe_(moon))</sup>(/ˈænθiː/, アンテ) is also known as Saturn XLIX, a very small natural satellite of Saturn, named after one of the Alkyonides; the name means flowery.
