# Changelog

## [0.11.0](https://github.com/0xwal/fusen.nvim/compare/v0.10.1...v0.11.0) (2026-08-30)


### ⚠ BREAKING CHANGES

* requires Neovim 0.8+ (uses vim.fs.normalize)

### Features

* add configurable spacing before EOL annotations ([#11](https://github.com/0xwal/fusen.nvim/issues/11)) ([e4d1cd5](https://github.com/0xwal/fusen.nvim/commit/e4d1cd52d9fddb0275697eecc90a5f7deee5df2d))
* add configurable telescope keymaps for mark deletion ([6e72dc1](https://github.com/0xwal/fusen.nvim/commit/6e72dc1fb7a67d9c40982d34b5da8b34da6a3ce0))
* add enable/disable/toggle commands for plugin control ([#20](https://github.com/0xwal/fusen.nvim/issues/20)) ([845ff1b](https://github.com/0xwal/fusen.nvim/commit/845ff1bd8c817e5a75c5af12ff841df58e863c35))
* add filetype-based keymap exclusion to avoid plugin conflicts ([84fa5b9](https://github.com/0xwal/fusen.nvim/commit/84fa5b91004e0896c418b82937258f47ef97542a))
* add FusenOpenSaveFile command ([9316851](https://github.com/0xwal/fusen.nvim/commit/93168519f0094fefbf226b495e6005df3cfe921f))
* improve extmark position tracking and change default keymap to ([b882881](https://github.com/0xwal/fusen.nvim/commit/b882881bf9953216d67fbf13be6ef5c877199a4d))
* Toggle mark (without confirmation) ([#27](https://github.com/0xwal/fusen.nvim/issues/27)) ([6a39bef](https://github.com/0xwal/fusen.nvim/commit/6a39bef8806bca0bfda8c20ec88a2843a2735e5c))
* **ui:** allow to add prefix :sparkles: ([bdb523d](https://github.com/0xwal/fusen.nvim/commit/bdb523d8f0ced2aea3abd487cf22cdb936594d0d))
* **ui:** allow to disable mark sign :sparkles: ([93295d5](https://github.com/0xwal/fusen.nvim/commit/93295d5ed2f22d6a2901d95c54c60cb7c9bc6851))
* yank marks to clipboard - hand your sticky notes to your AI assistant ([#29](https://github.com/0xwal/fusen.nvim/issues/29)) ([9df4900](https://github.com/0xwal/fusen.nvim/commit/9df4900d2b8f22406cf31b629457ca660fa00c1d))


### Bug Fixes

* change confirmation prompts to show default action (y/N) ([8abdb60](https://github.com/0xwal/fusen.nvim/commit/8abdb608b5922f64dd462417f06ed5a10995d035))
* clamp floating window column to non-negative values ([e64afdf](https://github.com/0xwal/fusen.nvim/commit/e64afdf1df2f22e7e16d72d53f2e8783c758c215))
* confirmation prompt format ([1cde60f](https://github.com/0xwal/fusen.nvim/commit/1cde60fd74f5ca2995906620079217b964c551d5))
* crash when opening floating window with long annotation ([a8d2bef](https://github.com/0xwal/fusen.nvim/commit/a8d2befcce900fe150ef5e322dd4cfae27c53261))
* float window positioning ([482580a](https://github.com/0xwal/fusen.nvim/commit/482580a8436a2c4b2ee1cf2e70c3e2c876ac09cc))
* improve float window height calculation with word wrapping ([c058440](https://github.com/0xwal/fusen.nvim/commit/c0584406e40e46156076d9fd81b0d8c1e5704976))
* mark search without buffer ([6fa1d68](https://github.com/0xwal/fusen.nvim/commit/6fa1d6828df677c5d2a45e83c16f3b6577f3a222))
* match telescope mark filtering against displayed text ([#34](https://github.com/0xwal/fusen.nvim/issues/34)) ([307f8f8](https://github.com/0xwal/fusen.nvim/commit/307f8f8e43202f1054f97655dd10b31892c51c58))
* prevent crash when rendering long annotations in floating window ([53685b3](https://github.com/0xwal/fusen.nvim/commit/53685b36ed6756ca0d722f7cc4b8a64b454881e5))
* refresh telescope picker after mark deletion and enable normal mode delete ([3ba94f9](https://github.com/0xwal/fusen.nvim/commit/3ba94f92e09f6ade29567f82d0fa8e4a7cc0df7e))
* scope mark list and yank to current project ([#33](https://github.com/0xwal/fusen.nvim/issues/33)) ([8fe941f](https://github.com/0xwal/fusen.nvim/commit/8fe941fbfa27b5aee2e219f9251b8db96deb776d))
* use nvim_win_text_height for exact float height ([#31](https://github.com/0xwal/fusen.nvim/issues/31)) ([bfb7de8](https://github.com/0xwal/fusen.nvim/commit/bfb7de8213387a40a0db4cae202ef49662274492))
* use strdisplaywidth instead of # to calculate message width ([9a28021](https://github.com/0xwal/fusen.nvim/commit/9a280218e42d4320a76e00b61f5c6f4f07327144))


### Performance Improvements

* reduce FocusGained delay by skipping unnecessary reloads ([#25](https://github.com/0xwal/fusen.nvim/issues/25)) ([7241461](https://github.com/0xwal/fusen.nvim/commit/72414619cc7ee91d562ca94c3778015104cbdbce))


### Documentation

* improve README screenshot table headers ([a4616a3](https://github.com/0xwal/fusen.nvim/commit/a4616a38590e82f6d3521979e0305069dcc5df03))
* unify configuration examples to use lazy.nvim syntax ([#13](https://github.com/0xwal/fusen.nvim/issues/13)) ([29ac230](https://github.com/0xwal/fusen.nvim/commit/29ac230358f1e86b791a7c28f146d004a94e83da))
* unify terminology and update media content ([#14](https://github.com/0xwal/fusen.nvim/issues/14)) ([fa8932c](https://github.com/0xwal/fusen.nvim/commit/fa8932c87fa3ed499280311b6f9f1ba35294d152))
* update exclude_filetypes examples in README ([44423fa](https://github.com/0xwal/fusen.nvim/commit/44423fa163698319d674b29d7c6309970fdfdcbb))
* update fusen.txt ([#24](https://github.com/0xwal/fusen.nvim/issues/24)) ([e2363a0](https://github.com/0xwal/fusen.nvim/commit/e2363a0f9ec0586332141c525250d889479a79b5))
* update README and help for telescope keymap configuration ([3e0cace](https://github.com/0xwal/fusen.nvim/commit/3e0caced2117d456f3b47b0273073a3da3e807ae))


### Miscellaneous Chores

* add release-please ([c3d8bf7](https://github.com/0xwal/fusen.nvim/commit/c3d8bf7d42df0a3b9cad5cb2abbe193c595aeea3))
* add release-please ([578ea99](https://github.com/0xwal/fusen.nvim/commit/578ea99d09051a3850edd4d1c5db9030f994e545))
* fix configs of release-please ([11f6a36](https://github.com/0xwal/fusen.nvim/commit/11f6a362bc01c97cbf7880bb15769400cd5fd15a))
* fix configs of release-please ([4e95cfb](https://github.com/0xwal/fusen.nvim/commit/4e95cfb00d907d507c25df4a4a1bd3ee2b6dc824))
* **main:** release 0.10.0 ([#32](https://github.com/0xwal/fusen.nvim/issues/32)) ([3dd46bc](https://github.com/0xwal/fusen.nvim/commit/3dd46bc031f54b0d3ab25a8edf81c3e2b825f294))
* **main:** release 0.10.1 ([#35](https://github.com/0xwal/fusen.nvim/issues/35)) ([2fd4e40](https://github.com/0xwal/fusen.nvim/commit/2fd4e40df111e1be0e49a232045df48839d734d0))
* **main:** release 0.5.1 ([#8](https://github.com/0xwal/fusen.nvim/issues/8)) ([5f5781d](https://github.com/0xwal/fusen.nvim/commit/5f5781d1dd715096150c0b842c4d172d2d7abef0))
* **main:** release 0.6.0 ([#12](https://github.com/0xwal/fusen.nvim/issues/12)) ([a4e2990](https://github.com/0xwal/fusen.nvim/commit/a4e2990b7ada2eb406de9d3440f6de7b946d90e8))
* **main:** release 0.6.1 ([#15](https://github.com/0xwal/fusen.nvim/issues/15)) ([f903a92](https://github.com/0xwal/fusen.nvim/commit/f903a9262aff5b462657351a9c7032b23f9bb2cd))
* **main:** release 0.7.0 ([#22](https://github.com/0xwal/fusen.nvim/issues/22)) ([40ff72e](https://github.com/0xwal/fusen.nvim/commit/40ff72e4289d4b894ad40f1d7a599840c23f03ad))
* **main:** release 0.7.1 ([#21](https://github.com/0xwal/fusen.nvim/issues/21)) ([ff57476](https://github.com/0xwal/fusen.nvim/commit/ff57476e167dd5437b6030616b7257e2a3b0619f))
* **main:** release 0.7.2 ([#26](https://github.com/0xwal/fusen.nvim/issues/26)) ([847cdb2](https://github.com/0xwal/fusen.nvim/commit/847cdb2f0ea49088e60bab848f4de510dc505521))
* **main:** release 0.8.0 ([#28](https://github.com/0xwal/fusen.nvim/issues/28)) ([4937374](https://github.com/0xwal/fusen.nvim/commit/4937374a5f37ae755d70d51595d40db04839b6a3))
* **main:** release 0.9.0 ([#30](https://github.com/0xwal/fusen.nvim/issues/30)) ([084edd0](https://github.com/0xwal/fusen.nvim/commit/084edd04b51231c6a1ab25f4c2f61681fe413089))


### Code Refactoring

* codes in marks.lua ([229f1b8](https://github.com/0xwal/fusen.nvim/commit/229f1b884a647da496f75c6710c553e76fe8a4b7))
* remove annotation prefix feature for simplicity ([0d861c7](https://github.com/0xwal/fusen.nvim/commit/0d861c73cc7fa6796b6dc5ce7b193699e8391b75))
* remove auto save config ([f77af6e](https://github.com/0xwal/fusen.nvim/commit/f77af6e153155bfaabebc5a054d3e7de3419f0c7))
* remove auto save config ([9dc7be5](https://github.com/0xwal/fusen.nvim/commit/9dc7be5fe9a8066ce340c99c568188e28a64305f))
* remove unnecessary codes ([eac3109](https://github.com/0xwal/fusen.nvim/commit/eac3109db284bea59cb150bfb590bd2e5b897016))
* remove unnecessary codes ([4e11c24](https://github.com/0xwal/fusen.nvim/commit/4e11c2408271e88cc4dc71503660642c1ecf3418))


### Continuous Integration

* skip tests for release-please PRs ([#18](https://github.com/0xwal/fusen.nvim/issues/18)) ([7a3b446](https://github.com/0xwal/fusen.nvim/commit/7a3b4463203dd9172f2eed44173926d3be36f3c4))

## [0.10.1](https://github.com/walkersumida/fusen.nvim/compare/v0.10.0...v0.10.1) (2026-07-22)


### Bug Fixes

* match telescope mark filtering against displayed text ([#34](https://github.com/walkersumida/fusen.nvim/issues/34)) ([307f8f8](https://github.com/walkersumida/fusen.nvim/commit/307f8f8e43202f1054f97655dd10b31892c51c58))

## [0.10.0](https://github.com/walkersumida/fusen.nvim/compare/v0.9.0...v0.10.0) (2026-07-19)


### ⚠ BREAKING CHANGES

* requires Neovim 0.8+ (uses vim.fs.normalize)

### Bug Fixes

* scope mark list and yank to current project ([#33](https://github.com/walkersumida/fusen.nvim/issues/33)) ([8fe941f](https://github.com/walkersumida/fusen.nvim/commit/8fe941fbfa27b5aee2e219f9251b8db96deb776d))
* use nvim_win_text_height for exact float height ([#31](https://github.com/walkersumida/fusen.nvim/issues/31)) ([bfb7de8](https://github.com/walkersumida/fusen.nvim/commit/bfb7de8213387a40a0db4cae202ef49662274492))

## [0.9.0](https://github.com/walkersumida/fusen.nvim/compare/v0.8.0...v0.9.0) (2026-07-12)


### Features

* yank marks to clipboard - hand your sticky notes to your AI assistant ([#29](https://github.com/walkersumida/fusen.nvim/issues/29)) ([9df4900](https://github.com/walkersumida/fusen.nvim/commit/9df4900d2b8f22406cf31b629457ca660fa00c1d))

## [0.8.0](https://github.com/walkersumida/fusen.nvim/compare/v0.7.2...v0.8.0) (2026-05-02)


### Features

* Toggle mark (without confirmation) ([#27](https://github.com/walkersumida/fusen.nvim/issues/27)) ([6a39bef](https://github.com/walkersumida/fusen.nvim/commit/6a39bef8806bca0bfda8c20ec88a2843a2735e5c))

## [0.7.2](https://github.com/walkersumida/fusen.nvim/compare/v0.7.1...v0.7.2) (2026-04-25)


### Performance Improvements

* reduce FocusGained delay by skipping unnecessary reloads ([#25](https://github.com/walkersumida/fusen.nvim/issues/25)) ([7241461](https://github.com/walkersumida/fusen.nvim/commit/72414619cc7ee91d562ca94c3778015104cbdbce))

## [0.7.1](https://github.com/walkersumida/fusen.nvim/compare/v0.7.0...v0.7.1) (2025-11-28)


### Documentation

* update fusen.txt ([#24](https://github.com/walkersumida/fusen.nvim/issues/24)) ([e2363a0](https://github.com/walkersumida/fusen.nvim/commit/e2363a0f9ec0586332141c525250d889479a79b5))


### Miscellaneous Chores

* **main:** release 0.7.0 ([#22](https://github.com/walkersumida/fusen.nvim/issues/22)) ([40ff72e](https://github.com/walkersumida/fusen.nvim/commit/40ff72e4289d4b894ad40f1d7a599840c23f03ad))

## [0.7.0](https://github.com/walkersumida/fusen.nvim/compare/v0.6.0...v0.7.0) (2025-11-15)


### Features

* add enable/disable/toggle commands for plugin control ([#20](https://github.com/walkersumida/fusen.nvim/issues/20)) ([845ff1b](https://github.com/walkersumida/fusen.nvim/commit/845ff1bd8c817e5a75c5af12ff841df58e863c35))


### Documentation

* unify terminology and update media content ([#14](https://github.com/walkersumida/fusen.nvim/issues/14)) ([fa8932c](https://github.com/walkersumida/fusen.nvim/commit/fa8932c87fa3ed499280311b6f9f1ba35294d152))


### Continuous Integration

* skip tests for release-please PRs ([#18](https://github.com/walkersumida/fusen.nvim/issues/18)) ([7a3b446](https://github.com/walkersumida/fusen.nvim/commit/7a3b4463203dd9172f2eed44173926d3be36f3c4))

## [0.6.1](https://github.com/walkersumida/fusen.nvim/compare/v0.6.0...v0.6.1) (2025-10-18)


### Documentation

* unify terminology and update media content ([#14](https://github.com/walkersumida/fusen.nvim/issues/14)) ([fa8932c](https://github.com/walkersumida/fusen.nvim/commit/fa8932c87fa3ed499280311b6f9f1ba35294d152))

## [0.6.0](https://github.com/walkersumida/fusen.nvim/compare/v0.5.1...v0.6.0) (2025-10-18)


### Features

* add configurable spacing before EOL annotations ([#11](https://github.com/walkersumida/fusen.nvim/issues/11)) ([e4d1cd5](https://github.com/walkersumida/fusen.nvim/commit/e4d1cd52d9fddb0275697eecc90a5f7deee5df2d))


### Documentation

* unify configuration examples to use lazy.nvim syntax ([#13](https://github.com/walkersumida/fusen.nvim/issues/13)) ([29ac230](https://github.com/walkersumida/fusen.nvim/commit/29ac230358f1e86b791a7c28f146d004a94e83da))

## [0.5.1](https://github.com/walkersumida/fusen.nvim/compare/v0.5.0...v0.5.1) (2025-09-13)


### Bug Fixes

* change confirmation prompts to show default action (y/N) ([8abdb60](https://github.com/walkersumida/fusen.nvim/commit/8abdb608b5922f64dd462417f06ed5a10995d035))
* confirmation prompt format ([1cde60f](https://github.com/walkersumida/fusen.nvim/commit/1cde60fd74f5ca2995906620079217b964c551d5))


### Miscellaneous Chores

* add release-please ([c3d8bf7](https://github.com/walkersumida/fusen.nvim/commit/c3d8bf7d42df0a3b9cad5cb2abbe193c595aeea3))
* add release-please ([578ea99](https://github.com/walkersumida/fusen.nvim/commit/578ea99d09051a3850edd4d1c5db9030f994e545))
* fix configs of release-please ([11f6a36](https://github.com/walkersumida/fusen.nvim/commit/11f6a362bc01c97cbf7880bb15769400cd5fd15a))
* fix configs of release-please ([4e95cfb](https://github.com/walkersumida/fusen.nvim/commit/4e95cfb00d907d507c25df4a4a1bd3ee2b6dc824))
