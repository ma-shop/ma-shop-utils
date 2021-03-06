# Common

### Steps to run locally on other apps.

Inside of this `common` project you need to run the following commands in terminal

```sh
make install # if you haven't already
make link-global # this links all the packages locally
make watch # watch for changes (this must be done before the next steps)
```

Inside the project you want to use these packages on you need to link the package you're updating and the main `@ma-shop/utils` package.

```sh
yarn link @ma-shop/[package] @ma-shop/utils
```

For example if you want to update the `@ma-shop/is` package you would run

```sh
yarn link @ma-shop/is @ma-shop/utils
```

- [x] @ma-shop/utils
  - [x] for all of these utils you would be able to access them through `@ma-shop/utils`
  - [x] export out lodash methods
    - `clamp`
    - `debounce`
    - `isEqual`
    - `pick`
    - `uniqueId`
    - `round`
    - `camelCase`
    - `kebabCase`
    - `lowerCase`
    - `snakeCase`
    - `startCase`
    - `upperCase`
  - [ ] ~~a way to set text components to be used in other utils~~
  - [x] `noop`, `noop.limit`
  - [x] `delay`
  - [x] `setEnv`
  - ~~`renderIf`~~
- [ ] @ma-shop/url (@ma-shop/shop-url?)
  - add different functions for modifying urls
  - add a function to set a way to modify the url each time so we can use `getTrackAndRedirectUrl` with it
  - add `open-url` functions
- [x] @ma-shop/is (this would go in the core)
- [x] @ma-shop/locale (this would go in the core)
  - a library to make dealing with locales easy
- [x] @ma-shop/files
  - this would be a rework of the index-files function make it more flexible
- [ ] ~~@ma-shop/analytics~~
  - ~~straight port of our current analytics (maybe @ma-shop/analytics-firebase)~~
- [ ] @ma-shop/address
  - building text addresses and react addresses
- [ ] @ma-shop/date
  - anything to do with dates (uses moment)
- [ ] @ma-shop/credit-cards
  - we only have a few of these but i'm sure we could add more
- [ ] @ma-shop/storage
  - rework our crucial-data to be more dynamic
- [ ] @ma-shop/haptic
- [ ] @ma-shop/navigation
- [ ] @ma-shop/spacing
  - add a way to configure the spacing
  - `noSpacing`, `noChildSpacing`, `noFirstChildSpacing`
- [ ] @ma-shop/font
  - add a way to set the default font size and the different settings(xl...)
  - `em`, `px`, `fontScale`
- [x] @ma-shop/react
  - `hoistStatic`, `setStateAsync`, `mapProps`, `setRef`, `interactions`, `renderIf`, `shapes`
- [ ] @ma-shop/react-native [includes @ma-shop/react]
  - add special is functions
- [ ] @ma-shop/share
- [ ] @ma-shop/translate
  - `t`
- [ ] @ma-shop/user (idk if this one is possible without reworking it)
- [ ] color (I'm adding this to my personal github)

* [ ] @ma-shop/components
