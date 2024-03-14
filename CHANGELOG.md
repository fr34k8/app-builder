# [4.2.0](https://github.com/develar/app-builder/compare/v3.4.2...v4.2.0) (2024-03-14)

## 5.0.0-alpha.0

### Major Changes

- [#107](https://github.com/develar/app-builder/pull/107) [`f4642dd`](https://github.com/develar/app-builder/commit/f4642ddcd85b482d1a7ed49f14d27c509eb5aa6b) Thanks [@mmaietta](https://github.com/mmaietta)! - chore: changing repo structure for release automation

### Minor Changes

- [#98](https://github.com/develar/app-builder/pull/98) [`3ed22df`](https://github.com/develar/app-builder/commit/3ed22df75fcff132a5b794ce1a421bec263bc118) Thanks [@yzewei](https://github.com/yzewei)! - feat: Add loongarch64 support

### Patch Changes

- [#106](https://github.com/develar/app-builder/pull/106) [`9704964`](https://github.com/develar/app-builder/commit/970496449b0b02780d654d61af1e3277515a2545) Thanks [@theogravity](https://github.com/theogravity)! - fix: Use npm config.mirror first before env variables for download URL

### Bug Fixes

- allow snapcraft version edge ([921a8e0](https://github.com/develar/app-builder/commit/921a8e0ec3c2515e669174a6895704c77c55b41f))
- Amazon S3 region detection seems to be broken ([05b559c](https://github.com/develar/app-builder/commit/05b559c28a782dfaf4b113b65cc8462fa5caa196)), closes [#22](https://github.com/develar/app-builder/issues/22) [#23](https://github.com/develar/app-builder/issues/23)
- binary plist to XMLFormat ([#34](https://github.com/develar/app-builder/issues/34)) ([b857403](https://github.com/develar/app-builder/commit/b85740334fec875f5dd8dcd22eb1f729599109db))
- check whole hashbang line if it is /usr/bin/env ([#66](https://github.com/develar/app-builder/issues/66)) ([e229f41](https://github.com/develar/app-builder/commit/e229f413d635b78a59b0d4ef1a9aa0f3967c0fd4))
- **deb:** remove gir1.2-gnomekeyring-1.0 package ([5768a76](https://github.com/develar/app-builder/commit/5768a760e60a1d3259684bb6f4636504507967b6))
- do not use ldflags for windows 386 due to false virus detection (size of exe increased from 13 to 18 MB) ([8e093d5](https://github.com/develar/app-builder/commit/8e093d59d0f63abe570726cbe9d11e7e72ee1a83)), closes [#33](https://github.com/develar/app-builder/issues/33)
- **download:** download failed when using ELECTRON_MIRROR ([#74](https://github.com/develar/app-builder/issues/74)) ([7e5f330](https://github.com/develar/app-builder/commit/7e5f3301fa7d517105276e7916db19d509eaa517))
- If downloading fails and a "custom" RootCA was declared in TLSClientConfig, retry download with default RootCA. ([#39](https://github.com/develar/app-builder/issues/39)) ([8bef6b3](https://github.com/develar/app-builder/commit/8bef6b342c1fb3c62cdc88cb03d491ddb8685cbf))
- instruct prebuild-install to download napi builds for dependencies which declare themselves to use napi ([#47](https://github.com/develar/app-builder/issues/47)) ([d8b8807](https://github.com/develar/app-builder/commit/d8b8807a11163974a27bc097b4e53c5445a5ca4e))
- **linux:** remove libappindicator-sharp from pacman dependency list ([#29](https://github.com/develar/app-builder/issues/29)) ([236a97a](https://github.com/develar/app-builder/commit/236a97a5773e48845367e4c399d20ec559fe5896))
- mac x64 arch ([04863f1](https://github.com/develar/app-builder/commit/04863f1bccccef97c95a544fe8ecd2ae743ca7cc))
- mksquashfs zstd support ([696179f](https://github.com/develar/app-builder/commit/696179f6ed2ee38d0ed000127bf4777e97e88e29))
- **node-modules:** incorrect generation of napi_versions ([#88](https://github.com/develar/app-builder/issues/88)) ([3b0c253](https://github.com/develar/app-builder/commit/3b0c253fa24a40f1904902dbb804ec23dc9ae4bf))
- not wrapping exec command with node unless it's a js file ([#44](https://github.com/develar/app-builder/issues/44)) ([014d570](https://github.com/develar/app-builder/commit/014d5703561049e3ff2d0d2f4365ed35b502675d))
- Return size info when converting icon ([#71](https://github.com/develar/app-builder/issues/71)) ([c92c3a2](https://github.com/develar/app-builder/commit/c92c3a2899b5887662321878a0a8681d122742bb)), closes [#42](https://github.com/develar/app-builder/issues/42)
- **snap:** remove incorrect usage of --target-arch for snapcraft ([#41](https://github.com/develar/app-builder/issues/41)) ([07239b5](https://github.com/develar/app-builder/commit/07239b565f9286fe7bdd65103ab61d5074c08b4c)), closes [#40](https://github.com/develar/app-builder/issues/40)
- Use 32-bit (ia32) app-builder.exe on Windows ARM64 ([#50](https://github.com/develar/app-builder/issues/50)) ([595bb30](https://github.com/develar/app-builder/commit/595bb30618dddf86e84fb11ccfc964354f2c7353))
- Use config.mirror first before env variables for download URL ([d45f97f](https://github.com/develar/app-builder/commit/d45f97f07b131a499a860bdc613c0119fdd924ec))

### Features

- add ability to set custom CA roots ([#28](https://github.com/develar/app-builder/issues/28)) ([47c3e0a](https://github.com/develar/app-builder/commit/47c3e0ace2f904f1431fa1fc57952f8ce6fefbe3))
- add env DISABLE_MULTIPART_DOWNLOADING to force downloading artifacts as one part ([4dbd42f](https://github.com/develar/app-builder/commit/4dbd42fea73c5d6526009de9d077375c46c0d41a))
- add Linux riscv64 support ([#90](https://github.com/develar/app-builder/issues/90)) ([4015728](https://github.com/develar/app-builder/commit/4015728d912d4c5483eb2942b8039c60de9631e9))
- add WSL (Windows Subsystem for Linux) support ([#21](https://github.com/develar/app-builder/issues/21)) ([1897b39](https://github.com/develar/app-builder/commit/1897b39c6d653a86e33aa01bfb046135761a0536))
- electron builder binaries base url from env ([#19](https://github.com/develar/app-builder/issues/19)) ([0f9fdf0](https://github.com/develar/app-builder/commit/0f9fdf0391b6950f2ea5f08cd05ef421c03c3e79))
- Handle symlinks, support pnpm and monorepo, ([#89](https://github.com/develar/app-builder/issues/89)) ([6c7d1e1](https://github.com/develar/app-builder/commit/6c7d1e12cec9c30ac851189822b0b34af194a56e))
- optionally support LZO compression for snap ([#65](https://github.com/develar/app-builder/issues/65)) ([4e5877e](https://github.com/develar/app-builder/commit/4e5877e254aef8fd933483ad94de55eca71d35d1))
- update zstd to 1.4.4 ([dfe6902](https://github.com/develar/app-builder/commit/dfe6902bd6d461e547c143c86af8540b03e9b55f))
- winCodeSign ([ad32971](https://github.com/develar/app-builder/commit/ad329712d9a22f7050d0040a4d427e16a40e3e6c))
- zstd 1.5.0, AppImage runtime 13, mksquashfs 4.5.0 with LZO and ZSTD support ([c24d1b5](https://github.com/develar/app-builder/commit/c24d1b50fbd313650ccab2021945eb006a39f0ae))
- zstd 1.5.5 (linux and windows) ([dadfa75](https://github.com/develar/app-builder/commit/dadfa75588e41ebd309f58b97e5e2e93065b5d06))
