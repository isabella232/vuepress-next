# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

# [2.0.0-beta.12](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.11...v2.0.0-beta.12) (2021-04-30)


### Bug Fixes

* **core:** avoid uri encoded filename ([4ff7f3b](https://github.com/vuepress/vuepress-next/commit/4ff7f3b287936cce0f9cfe5c8689c2efbb2b52aa))
* **theme-default:** align the font of line numbers with code blocks (close [#124](https://github.com/vuepress/vuepress-next/issues/124)) ([#125](https://github.com/vuepress/vuepress-next/issues/125)) ([a3ea87d](https://github.com/vuepress/vuepress-next/commit/a3ea87d507a644dc31bf9ffbb5703eb99342cc60))


### Features

* **core:** add deps to page object ([83c9aae](https://github.com/vuepress/vuepress-next/commit/83c9aaedcaf531d72d70ad514b9dd8ddf2e508d1))
* **core:** make filePath available in markdown env ([aa52549](https://github.com/vuepress/vuepress-next/commit/aa52549648b175626d3eafabe8629a78a8caf8e5))
* **markdown:** support import code blocks (close [#15](https://github.com/vuepress/vuepress-next/issues/15)) ([fe20ccc](https://github.com/vuepress/vuepress-next/commit/fe20cccf3d44565c7fcb890e8ebf2aa4659ab3e1))


### Performance Improvements

* **core:** reduce page data and component file size ([4c6eea5](https://github.com/vuepress/vuepress-next/commit/4c6eea5188e804cb3f6c7648d6528d43002618ae))
* **core:** reduce routes file size ([d926a17](https://github.com/vuepress/vuepress-next/commit/d926a170ee5f384845f5b166029fbc392f51dcde))


### BREAKING CHANGES

* **core:** `pagePath` prop of `<Content>` renamed to `pageKey`





# [2.0.0-beta.11](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.10...v2.0.0-beta.11) (2021-04-28)


### Bug Fixes

* **bundler-vite:** make the timestamp of client entry consistent ([4bbff4c](https://github.com/vuepress/vuepress-next/commit/4bbff4c22f67c456a0f4dcfe3ddf5724902a4d2a))


### Performance Improvements

* do not register hooks in dev mode for prod-only plugins ([d5af139](https://github.com/vuepress/vuepress-next/commit/d5af1398f059c075783c0c58456cef7b41bcaaf9))
* specify optimizeDeps for vite dev ([0d77331](https://github.com/vuepress/vuepress-next/commit/0d773312181380114cba16f61b633a5266dd1cf3))
* **core:** merge page routes to reduce requests in vite dev ([fa2a614](https://github.com/vuepress/vuepress-next/commit/fa2a61413c70afd426f74e57e6e5d2a4900c6568))





# [2.0.0-beta.10](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.9...v2.0.0-beta.10) (2021-04-27)


### Bug Fixes

* **bundler-vite:** avoid client code to be optimized or externalized ([f8a088d](https://github.com/vuepress/vuepress-next/commit/f8a088db5f428087a58dec4823627a9e3b447a75))
* **bundler-vite:** disable clearScreen in dev by default ([e7bfe49](https://github.com/vuepress/vuepress-next/commit/e7bfe49d10aa8d3c5121120435ed5076fbe80a27))
* **cli:** do not clean cache and temp on restart ([047a52c](https://github.com/vuepress/vuepress-next/commit/047a52c265db355de3aaa298c14150779e9182f4))
* **client:** implement ClientOnly correctly ([e27872d](https://github.com/vuepress/vuepress-next/commit/e27872d89f1e6894ebc734e2e26c800bea82e162))
* **client:** make hydration work properly (close [#123](https://github.com/vuepress/vuepress-next/issues/123)) ([34a5364](https://github.com/vuepress/vuepress-next/commit/34a5364ad6005e64a3e726296b9b8b73318fcbd4))
* **core:** allow extendsMarkdown to return a promise ([a4be2fd](https://github.com/vuepress/vuepress-next/commit/a4be2fda5952f64da2db6ba837b94bfb4e1315ce))


### Features

* **bundler-vite:** bump vite to 2.2.1 to support cacheDir ([d7f685b](https://github.com/vuepress/vuepress-next/commit/d7f685b5d729d9f8c9f858673355a37cb22fc90e))
* **client:** support custom layout ([c32866d](https://github.com/vuepress/vuepress-next/commit/c32866d769cb5a29fb811fd2f00e06d7b94e1508))
* **markdown:** support externalIcon in config and frontmatter ([#122](https://github.com/vuepress/vuepress-next/issues/122)) ([d1389bc](https://github.com/vuepress/vuepress-next/commit/d1389bc6c0eee3ad2fe83d5636fd293d0710e0fb))
* **plugin-search:** add search plugin (close [#35](https://github.com/vuepress/vuepress-next/issues/35)) ([70bb066](https://github.com/vuepress/vuepress-next/commit/70bb0668c53b984f17bdbf7b95ac8e3258034e73))
* **theme-default:** compat with docsearch and search plugin ([cb00182](https://github.com/vuepress/vuepress-next/commit/cb0018257c2c6b4b21e2add5f73e7213b537fb6f))
* **theme-default:** support pageClass frontmatter (close [#118](https://github.com/vuepress/vuepress-next/issues/118)) ([809d575](https://github.com/vuepress/vuepress-next/commit/809d5750c36662e894be566c0ff53c2f2a700da0))
* **theme-default:** support sidebarDepth ([b79ba90](https://github.com/vuepress/vuepress-next/commit/b79ba90f8e4cb93d76dac1f284131cf618aee784))





# [2.0.0-beta.9](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.8...v2.0.0-beta.9) (2021-04-21)


### Bug Fixes

* **core:** allow plugin itself as an item of plugin config array ([1fa8903](https://github.com/vuepress/vuepress-next/commit/1fa8903549d8f9eba3fc49e3117ee2018993b496))
* **core:** ensure trailing slash of page path (close [#114](https://github.com/vuepress/vuepress-next/issues/114)) ([cbcf166](https://github.com/vuepress/vuepress-next/commit/cbcf16624602e37c17935211ac4076c72db22507))
* **markdown:** do not escape extracted headers (close [#117](https://github.com/vuepress/vuepress-next/issues/117)) ([81b1336](https://github.com/vuepress/vuepress-next/commit/81b133622a00e6474f0bfe4a58e35bfab9fe3e49))
* **plugin-back-to-top:** fix back-to-top styles ([933643a](https://github.com/vuepress/vuepress-next/commit/933643aa9c24458eb914429b21f5ec22f6b23f9a))
* **theme-default:** remove font-smothing in code block ([41c281e](https://github.com/vuepress/vuepress-next/commit/41c281e016c77dc5f1d9d12e8917814e48af1424))


### Code Refactoring

* **core:** move evergreen option to bundler-webpack ([58c30c1](https://github.com/vuepress/vuepress-next/commit/58c30c1207f0f6e09e9d68096786ef189c67e9db))


### Features

* **client:** provide client types file ([89a32b5](https://github.com/vuepress/vuepress-next/commit/89a32b50767ef82556f5ae3300ec016e0acaf0e5))
* **core:** make frontmatter available in markdown env ([f977192](https://github.com/vuepress/vuepress-next/commit/f97719237db9d14c94716bf6b18fe52519a008cf))
* **plugin-palette:** add watchers for palette and style files ([0cf1b9b](https://github.com/vuepress/vuepress-next/commit/0cf1b9b346de2bc62789a940699298ee9e2873db))
* **plugin-register-components:** add register components plugin (close [#112](https://github.com/vuepress/vuepress-next/issues/112)) ([6af204d](https://github.com/vuepress/vuepress-next/commit/6af204df76b8f6969aef0fc061a64a796deb24ab))
* **theme-default:** add more palette variables for code styles ([db8e0f4](https://github.com/vuepress/vuepress-next/commit/db8e0f4870b051184a4d4b3c5b17497e302b0b11))


### BREAKING CHANGES

* **core:** `evergreen` option is moved to `bundlerConfig.evergreen` for bundler-webpack





# [2.0.0-beta.8](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.7...v2.0.0-beta.8) (2021-04-11)


### Bug Fixes

* **plugin-docsearch:** provide default value for locales (close [#107](https://github.com/vuepress/vuepress-next/issues/107)) ([491eb64](https://github.com/vuepress/vuepress-next/commit/491eb6416664775c366c0fb2a67388fe37098e2c))
* **plugin-pwa-popup:** provide default value for locales ([f7cbc15](https://github.com/vuepress/vuepress-next/commit/f7cbc15669c731e6598657c8048abe9cdfa4ee40))


### Code Refactoring

* normalize themes and plugins structure ([7781172](https://github.com/vuepress/vuepress-next/commit/77811722401bf1ed1fec44c64158ab0cd1ab3179))
* **core:** resolve theme when creating app ([fa683cb](https://github.com/vuepress/vuepress-next/commit/fa683cb76e8a3bcacc08d1dfd8bea6af79fee1d2))


### Features

* **markdown:** support internalTag option in links plugin ([1872ad9](https://github.com/vuepress/vuepress-next/commit/1872ad95d7c86247883c24f2ec86db07d7596923))
* **utils:** add logger.createError method ([0c198d7](https://github.com/vuepress/vuepress-next/commit/0c198d7f9e122828b37a2db670048cfc2ce20e81))


### BREAKING CHANGES

* client API that provided by plugins should be imported from `plugin-foo/lib/client`
* **core:** theme plugins could be overridden by user plugins now





# [2.0.0-beta.7](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.6...v2.0.0-beta.7) (2021-04-09)


### Bug Fixes

* **bundler-webpack:** always extract css file in build mode ([accc484](https://github.com/vuepress/vuepress-next/commit/accc484f95485a6013aad573f562565c16ac5ff8))
* **client:** install vue-router after clientAppEnhance (close [#100](https://github.com/vuepress/vuepress-next/issues/100)) ([2f5450f](https://github.com/vuepress/vuepress-next/commit/2f5450f0b8dcc4aa49b1c19a1adea6e84a1594c4))
* **client:** make page data hmr work as expected ([374ae43](https://github.com/vuepress/vuepress-next/commit/374ae43545c982ecc8762776035cc92359b874f5))
* **theme-default:** allow direct img children to be zoomable (close [#84](https://github.com/vuepress/vuepress-next/issues/84)) ([832bd6f](https://github.com/vuepress/vuepress-next/commit/832bd6fbbd9612e2209a28ed89a49bf9eb658838))


### Features

* **bundler-webpack:** bump webpack-dev-server to 4.0.0-beta.2 ([dd8c408](https://github.com/vuepress/vuepress-next/commit/dd8c40875cca382450d2758b2c7609bb69332d19))
* **core:** show warning when duplicate plugins are detected ([742f581](https://github.com/vuepress/vuepress-next/commit/742f5811032b3a2f0687edf3f966d25517734a8d))
* **plugin-toc:** add toc plugin ([0ea1720](https://github.com/vuepress/vuepress-next/commit/0ea1720ae3ed2007f0232123bfd7de77af6ae383))





# [2.0.0-beta.6](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.5...v2.0.0-beta.6) (2021-03-26)


### Reverts

* refactor(client): remove extra handling for router base ([6205279](https://github.com/vuepress/vuepress-next/commit/620527917e4d3ee7cfa4c1db7d3cadc36a30eaab))





# [2.0.0-beta.5](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.4...v2.0.0-beta.5) (2021-03-26)


### Bug Fixes

* **client:** ensure page component is loaded before route resolve ([598adf3](https://github.com/vuepress/vuepress-next/commit/598adf38b1f9edd3034bb011358a1a9d3bcb6b9e))
* **markdown:** avoid wrapping highlighted code with multiple pre ([f0b3872](https://github.com/vuepress/vuepress-next/commit/f0b38722f1a06c736366a36d7c4888952d28c947))
* **plugin-prismjs:** avoid loading languages multiple times ([4af5005](https://github.com/vuepress/vuepress-next/commit/4af50053c03408fc9e2e5426df89ae340de0e824))
* **theme-default:** add active class to sidebar group heading ([8dcb945](https://github.com/vuepress/vuepress-next/commit/8dcb9457c532de8076f94b3b165c1347e9bd9c86))
* **theme-default:** allow NavLink in sidebar children ([ea50010](https://github.com/vuepress/vuepress-next/commit/ea5001076b86a7dc8b807811796a8ed44fbcf7b9))
* **theme-default:** make navlink active in subpath (close [#70](https://github.com/vuepress/vuepress-next/issues/70)) ([4c865b1](https://github.com/vuepress/vuepress-next/commit/4c865b16430d0e72b0ac1103f9579a93f248bf9c))
* **theme-default:** make nested sidebar groups work ([4ada701](https://github.com/vuepress/vuepress-next/commit/4ada701062db400787c41008942354f6947bf80b))
* **theme-default:** make scrollBehavior work with transition (close [#77](https://github.com/vuepress/vuepress-next/issues/77)) ([4b8d0cf](https://github.com/vuepress/vuepress-next/commit/4b8d0cff2d7fa3d74d69d551976a3b12263e6124))


### Features

* **plugin-shiki:** add shiki plugin ([66bbcbd](https://github.com/vuepress/vuepress-next/commit/66bbcbde497cca525fc585b4046b11784e8d61bc))


### Performance Improvements

* improve HMR support ([38f0073](https://github.com/vuepress/vuepress-next/commit/38f007335864db4c9125ea5905ca91850fb7103b))





# [2.0.0-beta.4](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.3...v2.0.0-beta.4) (2021-03-20)


### Bug Fixes

* **bundler-vite:** disable auto resolving vite config file ([57967f7](https://github.com/vuepress/vuepress-next/commit/57967f7dec27c4148edf920decead327cc8746bf))


### Code Refactoring

* **markdown:** remove default syntax highlighter ([4a1abe3](https://github.com/vuepress/vuepress-next/commit/4a1abe39335eaaf3ef1dca3e35a324b12981c0d2))


### Features

* **plugin-prismjs:** add prismjs plugin ([638ad8a](https://github.com/vuepress/vuepress-next/commit/638ad8afdf9f3fe779e9eb1d02dca6c1caef0307))
* **theme-default:** use prismjs plugin ([f131de4](https://github.com/vuepress/vuepress-next/commit/f131de4783685dbabfde4e4966182d570224a246))


### BREAKING CHANGES

* **markdown:** prismjs is no longer the default syntax highlighter





# [2.0.0-beta.3](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.2...v2.0.0-beta.3) (2021-03-17)


### Bug Fixes

* **bundler-vite:** fix fs path on windows (close [#74](https://github.com/vuepress/vuepress-next/issues/74)) ([db3c3e8](https://github.com/vuepress/vuepress-next/commit/db3c3e8639d040aa8b408006d48b160a0b234e12))


### Features

* **cli:** show info of vite related packages ([73a66df](https://github.com/vuepress/vuepress-next/commit/73a66df2c19b4b292e5f7b48cb967490a0a5dd69))





# [2.0.0-beta.2](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.1...v2.0.0-beta.2) (2021-03-14)


### Bug Fixes

* **bundler-vite:** avoid optimizing client package ([5708934](https://github.com/vuepress/vuepress-next/commit/57089344f87bf381f8e6f2711eb6df9364c72432))
* **bundler-vite:** workaround for [vitejs/vite#2503](https://github.com/vitejs/vite/issues/2503) ([055b280](https://github.com/vuepress/vuepress-next/commit/055b280a8488c42614702533cc9eb8fb2852c71b))
* **plugin-nprogress:** always optimize nprogress with vite ([2aeb2bf](https://github.com/vuepress/vuepress-next/commit/2aeb2bf9b70b149bf2e56d2fd1b593e6628d72dd))





# [2.0.0-beta.1](https://github.com/vuepress/vuepress-next/compare/v2.0.0-beta.0...v2.0.0-beta.1) (2021-03-13)

**Note:** Version bump only for package vuepress-next





# [2.0.0-beta.0](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.26...v2.0.0-beta.0) (2021-03-13)


### Bug Fixes

* **plugin-google-analytics:** fix types ([92aa486](https://github.com/vuepress/vuepress-next/commit/92aa48629d0355808a15942594e499d39bb3f1e7))


### Features

* **vuepress-vite:** add vuepress-vite package ([03a6583](https://github.com/vuepress/vuepress-next/commit/03a658364d8c5f0b2510e10cd2bf8ec8bcbf41cb))
* implement vite hmr ([525c18d](https://github.com/vuepress/vuepress-next/commit/525c18d5a64fbdbdeb5ce1348ec1e1ead3dbd8f9))
* **bundler-vite:** add vite support :zap: ([7d612c4](https://github.com/vuepress/vuepress-next/commit/7d612c45d83d42b246316f93cc3385a9968307af))
* **cli:** add defineUserConfig util ([c20f7b7](https://github.com/vuepress/vuepress-next/commit/c20f7b7be5d04cb247d699c31bf6f68071180df6))
* **client:** add defineClientAppEnhance and defineClientAppSetup utils ([1520517](https://github.com/vuepress/vuepress-next/commit/15205172c3b56fc8a879bba040f4ecc815d2c924))
* **theme-default:** use sass as css pre-processor ([7eb1fd8](https://github.com/vuepress/vuepress-next/commit/7eb1fd8b8901d3f2c2335ad550b7d601a9354826))


### BREAKING CHANGES

* **theme-default:** the palette system of default theme is migrated to sass





# [2.0.0-alpha.26](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.25...v2.0.0-alpha.26) (2021-02-24)


### Bug Fixes

* **cli:** add theme-data plugin and rename palette plugin ([97ce42b](https://github.com/vuepress/vuepress-next/commit/97ce42bddbfcef5e66476c2355e031e54d9176ea))


### Features

* **bundler-webpack:** enable options API by default ([e29b6e1](https://github.com/vuepress/vuepress-next/commit/e29b6e1bb1ba89b7d440e54dafe3a84ecf4273db))
* **plugin-palette:** add palette plugin ([556a23c](https://github.com/vuepress/vuepress-next/commit/556a23cc9076f972deb3d5c0905441b63b700682))


### BREAKING CHANGES

* **plugin-palette:** migrate `@vuepress/plugin-palette-stylus` to `@vuepress/plugin-palette`





# [2.0.0-alpha.25](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.24...v2.0.0-alpha.25) (2021-02-20)


### Bug Fixes

* **markdown:** do not treat autolink as a component (close [#60](https://github.com/vuepress/vuepress-next/issues/60)) ([9f6cffa](https://github.com/vuepress/vuepress-next/commit/9f6cffa1e0c39d0caf9f7ab34c5f06f36a87948b))


### Code Refactoring

* **core:** remove theme data from site data ([187aef3](https://github.com/vuepress/vuepress-next/commit/187aef36607efc62d7b2d5c773553f89685cf64c))


### Features

* **plugin-theme-data:** extract theme data injection to a plugin ([e971e39](https://github.com/vuepress/vuepress-next/commit/e971e3964cf11361ac267501768b0f8bc7dba909))


### BREAKING CHANGES

* **core:** `themeConfig` is not available in site data any more





# [2.0.0-alpha.24](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.23...v2.0.0-alpha.24) (2021-02-13)


### Code Refactoring

* **core:** change page default date to 0000-00-00 ([1ce602e](https://github.com/vuepress/vuepress-next/commit/1ce602ef811f29f083a8d10695a7b212ed82cae5))
* **core:** remove permalink and pattern from page options ([9534989](https://github.com/vuepress/vuepress-next/commit/9534989a82e620b1c09b4a09d4cfee1e99d145fc))


### Features

* **core:** add extendsPageOptions hook ([19b7e83](https://github.com/vuepress/vuepress-next/commit/19b7e83cb25ec523857d34c415782d595a05d0ff))
* **core:** add watchers parameter to onWatched hook ([0bcd594](https://github.com/vuepress/vuepress-next/commit/0bcd594d1645fe9994d1456e86803e5619057bfb))


### BREAKING CHANGES

* **core:** remove permalink and pattern from page options
* **core:** change page default date from 1970-01-01 to 0000-00-00





# [2.0.0-alpha.23](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.22...v2.0.0-alpha.23) (2021-02-10)


### Bug Fixes

* **markdown:** remove site base from internal links (close [#58](https://github.com/vuepress/vuepress-next/issues/58)) ([a8c7fdd](https://github.com/vuepress/vuepress-next/commit/a8c7fdd86a9c4f08c51673f3dba0451455a731d2))





# [2.0.0-alpha.22](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.21...v2.0.0-alpha.22) (2021-02-10)


### Bug Fixes

* **client:** only watch route path to update head ([3174f5a](https://github.com/vuepress/vuepress-next/commit/3174f5a676d95943df256b2be31227eb844d0144))
* **plugin-debug:** avoid enabling in production mode (close [#53](https://github.com/vuepress/vuepress-next/issues/53)) ([9612282](https://github.com/vuepress/vuepress-next/commit/961228234e3983f1f84f992a1317316d09f8cb98))





# [2.0.0-alpha.21](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.20...v2.0.0-alpha.21) (2021-02-05)


### Features

* **plugin-git:** collect page created time (close [#45](https://github.com/vuepress/vuepress-next/issues/45)) ([4045a8c](https://github.com/vuepress/vuepress-next/commit/4045a8c1ab591dbbb0303aa43c6d13bf248d995c))


* **plugin-google-analytics:** migrate to google analytics 4 (close [#36](https://github.com/vuepress/vuepress-next/issues/36)) ([d2393f7](https://github.com/vuepress/vuepress-next/commit/d2393f7970c346bfcef2e72658f9a4a89a93b396))


### BREAKING CHANGES

* migrate to google analytics 4 and drop v3 support





# [2.0.0-alpha.20](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.19...v2.0.0-alpha.20) (2021-02-04)


### Bug Fixes

* **plugin-medium-zoom:** always refresh medium-zoom with delay ([2495f5d](https://github.com/vuepress/vuepress-next/commit/2495f5d30fa75b50c203919abf2d8dab7dfda2d9))
* **theme-default:** fix max width of navbar links wrapper ([846e60c](https://github.com/vuepress/vuepress-next/commit/846e60ca9f0137f54a96df7589df4ea4cd99f18a))
* **theme-default:** remove extra rem in styles (close [#50](https://github.com/vuepress/vuepress-next/issues/50)) ([9b1b852](https://github.com/vuepress/vuepress-next/commit/9b1b852a9c11c28b43253f87b40362693ad2cb95))


### Features

* **core:** create siteData in vuepress app ([05b87dd](https://github.com/vuepress/vuepress-next/commit/05b87ddf32f32c94cc131e0074365aeba70f85f2))
* **core:** make language available in page data ([03bb09f](https://github.com/vuepress/vuepress-next/commit/03bb09fd51aeaff56d26820a1401b87ea8bdeb38))





# [2.0.0-alpha.19](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.18...v2.0.0-alpha.19) (2021-01-24)


### Bug Fixes

* **cli:** add esbuild external ([8d285ea](https://github.com/vuepress/vuepress-next/commit/8d285ea88946683d96d46a379d4215963338dff4))


### Features

* **core:** add onWatched hook ([9725a10](https://github.com/vuepress/vuepress-next/commit/9725a101599363094a85916317109b67d365dff4))
* **plugin-docsearch:** allow more fields in locales config ([ce1cf18](https://github.com/vuepress/vuepress-next/commit/ce1cf18248129f44651b33091329c4366320131b))





# [2.0.0-alpha.18](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.17...v2.0.0-alpha.18) (2021-01-17)


### Bug Fixes

* **client:** load existing head tags on mounted ([15722c5](https://github.com/vuepress/vuepress-next/commit/15722c5175e44a8d6363bfe5f138f2c2c8edeec3))
* **markdown:** load some languages by default to partially avoid prism issue ([48c085a](https://github.com/vuepress/vuepress-next/commit/48c085af6a8751211fe7180a82bb67ff5a7b191f))
* **theme-default:** fix homepage frontmatter type ([9cf2d28](https://github.com/vuepress/vuepress-next/commit/9cf2d288e115d335f6ff9f1a849a2ce82db799c9))
* **theme-default:** fix sidebar config override ([2c2c280](https://github.com/vuepress/vuepress-next/commit/2c2c2801be716dfb102345090888fd1e22a0ac92))
* **theme-default:** make sr-only tags unselectable ([0f6488e](https://github.com/vuepress/vuepress-next/commit/0f6488e3a00674c0670737c8831763db0a0ffa93))


### Features

* **client:** make usePageFrontmatter generic ([2c5e5c1](https://github.com/vuepress/vuepress-next/commit/2c5e5c1400469a3cb4da2856104514a9413bff8a))
* **shared:** optimize frontmatter type and support generics ([8a7025f](https://github.com/vuepress/vuepress-next/commit/8a7025ff39b4656f98f9a35e93848373ce72ddbe))
* **theme-default:** add code-group custom container ([d0a20aa](https://github.com/vuepress/vuepress-next/commit/d0a20aaacefc78708a4181c53704b28c60b520b4))
* **theme-default:** add page transition ([845cc2c](https://github.com/vuepress/vuepress-next/commit/845cc2cb64223b856261bfc7b384dec6557456c4))
* **theme-default:** allow html in homepage footer ([87e0821](https://github.com/vuepress/vuepress-next/commit/87e0821cee66c34141c1c3a62e8f5ecb6b21a957))
* **theme-default:** optimize scrollbar style of sidebar ([27abb26](https://github.com/vuepress/vuepress-next/commit/27abb26509fa737ea27c3036bbe834d544e60298))
* **theme-default:** support multiple action buttons in homepage (close [#23](https://github.com/vuepress/vuepress-next/issues/23)) ([bb44710](https://github.com/vuepress/vuepress-next/commit/bb44710624d2dbb65bd5f3da2eafabdec73ecadf))





# [2.0.0-alpha.17](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.16...v2.0.0-alpha.17) (2021-01-13)


### Bug Fixes

* **bundler-webpack:** add trailing slash to url ([cbe4c7f](https://github.com/vuepress/vuepress-next/commit/cbe4c7f3924c11b751dfefbb01f8fc0528516b3b))


### Features

* **cli:** add --clean-temp option ([752d725](https://github.com/vuepress/vuepress-next/commit/752d72563d88d5441a5570af3bc1b4c571e268c2))
* **theme-default:** allow dropdown subtitle as a link ([5fb6558](https://github.com/vuepress/vuepress-next/commit/5fb6558c926ddbb569f2b1901903cf9be4ad426e))





# [2.0.0-alpha.16](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.15...v2.0.0-alpha.16) (2021-01-11)


### Bug Fixes

* **core:** support special characters in filename and permalink ([c3e68ef](https://github.com/vuepress/vuepress-next/commit/c3e68ef6a4aa3f6722d5bc4079bafe5d3b176e5e))
* **markdown:** fix assets relative path handling (close [#33](https://github.com/vuepress/vuepress-next/issues/33)) ([9a95431](https://github.com/vuepress/vuepress-next/commit/9a95431aa3994855f7194d3efe810b4fd2cf72d9))


### Features

* **cli:** show info of vue packages ([2d19e84](https://github.com/vuepress/vuepress-next/commit/2d19e84c1ac24e1a127d330009617c42eb7a2bc3))





# [2.0.0-alpha.15](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.14...v2.0.0-alpha.15) (2021-01-04)


### Bug Fixes

* **core:** fix site locale data type ([7898500](https://github.com/vuepress/vuepress-next/commit/7898500f8b611662777ca3bdeb89c5b3bb658595))
* **theme-default:** click to close dropdown that opened by tab and click ([88d1ae2](https://github.com/vuepress/vuepress-next/commit/88d1ae2bf6a92113ece8efa7ed57352b34ad18c4))
* **theme-default:** fix font-size of dropdown group title ([563156c](https://github.com/vuepress/vuepress-next/commit/563156cb8458aeb71fadd882b08e03bee8ae5fba))


### Features

* **core:** provide app in all plugin hooks ([21cc3a6](https://github.com/vuepress/vuepress-next/commit/21cc3a608e54d38de8de8f453b5e88031b4cedb1))


### Reverts

* fix(theme-default): remove outline when focused on dropdown button ([66d3feb](https://github.com/vuepress/vuepress-next/commit/66d3feba01bf8a3ce751788a9a025dd69757efb4))





# [2.0.0-alpha.14](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.13...v2.0.0-alpha.14) (2021-01-03)


### Bug Fixes

* **bundler-webpack:** remove esbuild minimizer ([4b3c00b](https://github.com/vuepress/vuepress-next/commit/4b3c00becad376fed98bfaef700e565c19724a0b))
* **core:** fix page date resolving ([de6c5c8](https://github.com/vuepress/vuepress-next/commit/de6c5c8ca89347bea4ba2925e283a7b710a5b5d3))
* **plugin-docsearch:** fix docsearch style issue ([7550587](https://github.com/vuepress/vuepress-next/commit/7550587dbdf876b834dc14aa83847fabf1dba668))
* **theme-default:** assign default locale data ([d59f55d](https://github.com/vuepress/vuepress-next/commit/d59f55d355299a8edbdb43986cc7aaff5345ea1f))
* **theme-default:** fix overflow style of code block line-numbers ([dd77cf4](https://github.com/vuepress/vuepress-next/commit/dd77cf448a28423ee23930b3d76601d8a5a6da18))
* **theme-default:** remove outline when focused on dropdown button ([77842e3](https://github.com/vuepress/vuepress-next/commit/77842e396f1ebcc9e874af537a6520b818d028c2))
* **theme-default:** set font-size explicitly for h4 to h6 ([a6459c0](https://github.com/vuepress/vuepress-next/commit/a6459c0eca38fbc19545442581ea6f0e73908b30))
* **vuepress:** add a wrapper for cli bin (close [#21](https://github.com/vuepress/vuepress-next/issues/21)) ([2708ac3](https://github.com/vuepress/vuepress-next/commit/2708ac325c05a39cc5139e7e5f902e2fead5ca7a))





# [2.0.0-alpha.13](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.12...v2.0.0-alpha.13) (2020-12-23)


### Bug Fixes

* **markdown:** only prepend prefix to explicit relative image path ([8d6a095](https://github.com/vuepress/vuepress-next/commit/8d6a095ace0ed724b4ac4eea0e44a28f120a48bc))
* **plugin-git:** replace -P with --no-pager for better compatibility (close [#16](https://github.com/vuepress/vuepress-next/issues/16)) ([f394c78](https://github.com/vuepress/vuepress-next/commit/f394c78a06a3dae7cea91759db6010d04746f999))


### Features

* **cli:** respect conventional clientAppEnhance files (close [#20](https://github.com/vuepress/vuepress-next/issues/20)) ([0777376](https://github.com/vuepress/vuepress-next/commit/0777376bcb5cafec50f47877a6bf3926d6ff0076))





# [2.0.0-alpha.12](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.11...v2.0.0-alpha.12) (2020-12-19)


### Bug Fixes

* **markdown:** support v-on shorthand in html inline tags ([86a1299](https://github.com/vuepress/vuepress-next/commit/86a1299d16555fb453f36aa1db49ff9ce184e874))
* **theme-default:** fix navbar type to allow nested group ([9ef46ae](https://github.com/vuepress/vuepress-next/commit/9ef46ae3d41dc56c536d884665d28f71a7883a59))


### Features

* **markdown:** code-block-level config for line-numbers and v-pre ([9ac3e4a](https://github.com/vuepress/vuepress-next/commit/9ac3e4a12066f8b05e5d3a5211adf837a944c29d))





# [2.0.0-alpha.11](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.10...v2.0.0-alpha.11) (2020-12-17)


### Bug Fixes

* **bundler-webpack:** freeze webpack version ([95523a2](https://github.com/vuepress/vuepress-next/commit/95523a2f2b32f8dad773c74553bd22a0940cd27a))





# [2.0.0-alpha.10](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.9...v2.0.0-alpha.10) (2020-12-17)


### Bug Fixes

* **theme-default:** fix content headers styles ([7ead1f6](https://github.com/vuepress/vuepress-next/commit/7ead1f60db5135ed7d1a428cb23fecbbc11b223e))


### Features

* **cli:** add info command ([1f30993](https://github.com/vuepress/vuepress-next/commit/1f30993a920189c0de89e413d85feb957546e47f))





# [2.0.0-alpha.9](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.8...v2.0.0-alpha.9) (2020-12-16)


### Bug Fixes

* **bundler-webpack:** freeze version of prerelease packages ([50d5fa0](https://github.com/vuepress/vuepress-next/commit/50d5fa0b88cfdf1924a38cbc0d19d29ce2bdef89))
* **cli:** prepare pages entry if the page key is changed ([4c79839](https://github.com/vuepress/vuepress-next/commit/4c79839b730dd9cd9042c5929820d09ce102a88f))
* **plugin-git:** split arguments to get updated time ([70e8b5e](https://github.com/vuepress/vuepress-next/commit/70e8b5ec0e7a960ef9a2398200ff23ae67086ab9))





# [2.0.0-alpha.8](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.7...v2.0.0-alpha.8) (2020-12-11)


### Bug Fixes

* **bundler-webpack:** display localhost by default in console ([8bf0987](https://github.com/vuepress/vuepress-next/commit/8bf0987b71588b2959475da9d502b2e4f9cc6bbb))
* **cli:** remove shorthand of host option ([8340797](https://github.com/vuepress/vuepress-next/commit/8340797da03462c8078753a4535a9977c349ca04))


### Features

* **plugin-pwa:** migrate pwa plugin ([aa54fd6](https://github.com/vuepress/vuepress-next/commit/aa54fd65aa77b32b97de0a38359f1ad07f96f566))
* **plugin-pwa-popup:** extract pwa popup plugin ([c3e8fb2](https://github.com/vuepress/vuepress-next/commit/c3e8fb26c348b7cae47f7cc0c4a0fba998c308d3))





# [2.0.0-alpha.7](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.6...v2.0.0-alpha.7) (2020-12-09)


### Bug Fixes

* **bundler-webpack:** fix windows compatibility (close [#12](https://github.com/vuepress/vuepress-next/issues/12)) ([f35f768](https://github.com/vuepress/vuepress-next/commit/f35f76861785e69c26d3e8731d5a1afe7e2f01be))





# [2.0.0-alpha.6](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.5...v2.0.0-alpha.6) (2020-12-09)


### Features

* **bundler-webpack:** migrate to webpack 5 ([37dca96](https://github.com/vuepress/vuepress-next/commit/37dca9644622a61e50ba2cda420c08581a824a19))
* **client:** remove built-in debug component ([a5962bb](https://github.com/vuepress/vuepress-next/commit/a5962bb82483f56800b33b4e35c50dcb49fd48b1))
* **plugin-debug:** add debug plugin ([ddf0a92](https://github.com/vuepress/vuepress-next/commit/ddf0a925c849fd7dba894ee69f9840d63dee99f4))
* **shared:** add esm build ([f8463e7](https://github.com/vuepress/vuepress-next/commit/f8463e791c909493e343d98468663c9d31bcbb5f))
* **theme-default:** use debug plugin ([e12b1f3](https://github.com/vuepress/vuepress-next/commit/e12b1f3293b5e8faebd93b444b71b6ac11b1029d))





# [2.0.0-alpha.5](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.4...v2.0.0-alpha.5) (2020-12-03)


### Bug Fixes

* **plugin-google-analytics:** report site base ([31c8cad](https://github.com/vuepress/vuepress-next/commit/31c8cadfba7676e7ac5809d669a6262f421e7831))
* **theme-default:** fix code related styles ([83d8a6f](https://github.com/vuepress/vuepress-next/commit/83d8a6f50537ed1b4c5e5c0f4221841999eeaeab))
* **theme-default:** fix the condition of using router-link as nav-link ([8141f69](https://github.com/vuepress/vuepress-next/commit/8141f691495fc92ee19bd4d7bfd496c07112ac6a))


### Features

* **markdown:** support doc lang highlight ([dc91db6](https://github.com/vuepress/vuepress-next/commit/dc91db6327fd818f365abbec96cc5dde0b6ba243))





# [2.0.0-alpha.4](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.3...v2.0.0-alpha.4) (2020-12-02)


### Bug Fixes

* **bundler-webpack:** remove spinner when preparing data ([7f3b425](https://github.com/vuepress/vuepress-next/commit/7f3b4253a6d4d2f58b3487a407c609c417be1326))
* **cli:** keep message format consistent ([1de416d](https://github.com/vuepress/vuepress-next/commit/1de416d75fb115523d78e6e709712210cbf39db9))
* **core:** failed to resolve local theme ([4d836e2](https://github.com/vuepress/vuepress-next/commit/4d836e2bc3e7affe17f63df1c4ce40c464a7e6fb))
* **core:** warn if layout directory does not exist ([3d2d414](https://github.com/vuepress/vuepress-next/commit/3d2d4148024963521b9e1ebbc29aa19697ac3452))


### Features

* **cli:** allow default export in user config file ([b2f86c7](https://github.com/vuepress/vuepress-next/commit/b2f86c7b6c11de81c5aaf6e96973921dc0b9ad60))
* **cli:** allow loading ts files globally ([a9d94ac](https://github.com/vuepress/vuepress-next/commit/a9d94ac9243ec75c5de20a0a08546e3a032dd43e))
* **utils:** add hasExportDefault util ([575a9c5](https://github.com/vuepress/vuepress-next/commit/575a9c5d9eee44c0ce20b0712830e2eb2a303780))





# [2.0.0-alpha.3](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.2...v2.0.0-alpha.3) (2020-12-01)


### Bug Fixes

* **bundler-webpack:** check public dir before using copy-plugin ([2481802](https://github.com/vuepress/vuepress-next/commit/248180221e870a2e1cc2e4a67973c4e0918a3651))
* **core:** avoid runtime warning for empty template (close [#10](https://github.com/vuepress/vuepress-next/issues/10)) ([bcbf703](https://github.com/vuepress/vuepress-next/commit/bcbf703e6e449f7753697b7dfc503bd643bfd240))


### Features

* **cli:** use esbuild to load ts file ([41cfbc5](https://github.com/vuepress/vuepress-next/commit/41cfbc57872f00b1f8ff80ffc9b127942792fbc6))





# [2.0.0-alpha.2](https://github.com/vuepress/vuepress-next/compare/v2.0.0-alpha.1...v2.0.0-alpha.2) (2020-12-01)


### Bug Fixes

* **plugin-git:** check if git repo is valid ([3e9fc83](https://github.com/vuepress/vuepress-next/commit/3e9fc8301e3fc9a0be7a8c7ede25e10063a10c9f))


### Features

* **bundler-webpack:** use esbuild for compilation and minification ([4351f99](https://github.com/vuepress/vuepress-next/commit/4351f997ffee41d560a257abd28880aa98ee29a4))





# 2.0.0-alpha.1 (2020-12-01)
