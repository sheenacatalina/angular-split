<a name="14.1.0"></a>

# 14.1.0 (2022-09-11)

- **fix** spurious network call due to empty background image [#322](https://github.com/angular-split/angular-split/pull/322) thanks to [rahuldimri](https://github.com/rahuldimri)!

<a name="14.0.0"></a>

# 14.0.0 (2022-07-18)

- **Chore** add support for Angular 14

<a name="13.2.0"></a>

# 13.2.0 (2022-02-13)

- **Feat** add keyboard accessibility [#317](https://github.com/angular-split/angular-split/pull/317) thanks to [dxbrandon](https://github.com/dxbrandon)!

<a name="13.1.0"></a>

# 13.1.0 (2021-11-26)

- **Feat** allow for setting global config (issue [#166](https://github.com/angular-split/angular-split/issues/166) / PR [#309](https://github.com/angular-split/angular-split/pull/309)) thanks to [pawelwojkiewicz](https://github.com/pawelwojkiewicz).

<a name="13.0.1"></a>

# 13.0.1 (2021-11-20)

- **Fix** export internal interfaces (issue [#307](https://github.com/angular-split/angular-split/issues/307)).

<a name="13.0.0"></a>

# 13.0.0 (2021-11-20)

- **Chore** add support for Angular 13

<a name="5.0.0"></a>

# 5.0.0 (2020-12-18)

- **Fix** fire dragStart event only when a cursor is moved [#283](https://github.com/angular-split/angular-split/issues/283) thanks to [nomeaning777](https://github.com/nomeaning777)!

<a name="5.0.0-beta.2"></a>

# 5.0.0-beta.2 (2020-11-23)

- **Feat** Add Expand/Collapse functionality [#276](https://github.com/angular-split/angular-split/issues/276) thanks to [Shemesh](https://github.com/Shemesh)!
- **Chore** Update project to Angular 11 [#278](https://github.com/angular-split/angular-split/issues/278)

<a name="5.0.0-beta.1"></a>

# 5.0.0-beta.1 (2020-09-06)

- **Fix** Make type of gutterSize getter/setter consistent

<a name="5.0.0-beta.0"></a>

# 5.0.0-beta.0 (2020-08-30)

- **Chore** Update project to Angular 10 [#256](https://github.com/angular-split/angular-split/issues/256) thanks to [greggbjensen](https://github.com/greggbjensen)!

<a name="4.0.0"></a>

# 4.0.0 (2020-07-24)

- **Release** release version 4.0.0

<a name="4.0.0-beta.1"></a>

# 4.0.0-beta.1 (2020-07-23)

- **Fix** fix: undefined errors in access-from-class demo [#247](https://github.com/angular-split/angular-split/issues/247).

<a name="4.0.0-beta.0"></a>

# 4.0.0-beta.0 (2020-07-23)

- **Fix** More precise type for AngularSplitModule [#204](https://github.com/angular-split/angular-split/issues/204).
- **Fix** export IOutputData and IOutputAreaSizes interfaces [#226](https://github.com/angular-split/angular-split/issues/226).
- **Fix** Wait for drag-end post-processing before starting next drag [#217](https://github.com/angular-split/angular-split/issues/217).
- **Fix** Fix styles lost when hosting application set to ViewEncapsulation.None [#177](https://github.com/angular-split/angular-split/issues/177).
- **Chore** Fix travis tests [#221](https://github.com/angular-split/angular-split/issues/221).
- **Chore** Configure prettier, husky and lint-staged [#243](https://github.com/angular-split/angular-split/issues/243).
- **Chore** Update docs, sort properties alphabetically, document 'order' property [#245](https://github.com/angular-split/angular-split/issues/245).

<a name="3.0.3"></a>

# 3.0.3 (2020-02-13)

- **Angular version upgrade:** Update `package.json` peerDependancies versions to allow Angular 9 [#218](https://github.com/angular-split/angular-split/issues/218).

<a name="3.0.2"></a>

# 3.0.2 (2019-06-22)

- **Angular version upgrade:** Add support for Angular 8 [#175](https://github.com/angular-split/angular-split/issues/175).

<a name="3.0.1"></a>

# 3.0.1 (2019-05-07)

- **Bug:** Fix `(dragEnd)` event which was emitted outside zone [#172](https://github.com/angular-split/angular-split/issues/171).

<a name="3.0.0"></a>

# 3.0.0 (2019-05-06)

- **Pixel mode:** Now your can choose to work with `pixel` or `percent` mode. In `pixel` mode, an area with wildcard size (`size="*"`) is mandatory.
- **minSize & maxSize area:** Now you can set minimum and maximum sizes for each areas whatever the current mode (Only exception is the wildcard area size in `pixel` mode, no min/max allowed for it).
- **lockSize area:** Use `<as-split-area [size]="X" [lockSize]="true">` as a shortcut for `<as-split-area [size]="X" [minSize]="X" [maxSize]="X">`.
- **gutterDblClick event:** Double click on gutter is now catchable with `(gutterDblClick)`.
- **gutterDblClickDuration property:** Specify duration between 2 clicks to consider a double click `(gutterDblClick)` event.
- **exportAs:** You can access `SplitComponent` as `<as-split #split="asSplit">` and `SplitAreaDirective` as `<as-split-area #area1="asSplitArea">` from template variables easily using `ViewChild` decorator.
- **CSS classes updates:** Some `split`, `area` and `gutter` elements has CSS class names updates, check documentation.
- **Internal:** Remove `EventManagerPlugin` and start/end/click subscribers stuff which was added to avoid some change detection runs but adding too much complexity.. I stopped going against the framework, clearer now and works better with lazy loaded modules!

<a name="2.0.1"></a>

# 2.0.1 (2018-12-21)

- **Module import:** Service now provided inside `AngularSplitModule.forRoot()` method instead of directly in module annotation. _Warning: Be sure to import module using `forRoot()` method otherwise it will not works anymore._
- **Internal:** Now use an `EventManagerPlugin` instead of extending `EventManager` and use "as-split-undetected." template event prefix.

<a name="2.0.0"></a>

# 2.0.0 (2018-12-09)

- **New major version:** Check previous betas to know main changes from `1.x` and take a look on website examples.

<a name="2.0.0-beta.8"></a>

# 2.0.0-beta.8 (2018-12-06)

- **New gutter css class:** CSS class `is-dragged` added on the gutter while being dragged.

<a name="2.0.0-beta.7"></a>

# 2.0.0-beta.7 (2018-12-05)

- **New API:** Add `getVisibleAreaSizes(): Array<number>` function on `SplitComponent` class.

<a name="2.0.0-beta.6"></a>

# 2.0.0-beta.6 (2018-12-03)

- **Internal:** Use `clientX`/`clientY` instead `pageX`/`pageY` to calculate distance while mouse moves.

<a name="2.0.0-beta.5"></a>

# 2.0.0-beta.5 (2018-11-29)

- **Performance:** Make library template event bindings (`click`, `mousedown`, `touchstart`) runs outside `zone.js` to avoid unnecessary change detection run.
- **Performance (API change):** Remove `(dragProgress)` event emitter from template and add a `dragProgress$` observable accessible from `SplitComponent` class. Doing this you can track drag progress without triggering change detection inside component containing `<as-split>`, see "Sync example demo" opening devTools console to verify it.
- **New API:** Add `setVisibleAreaSizes(sizes: Array<number>): boolean` function on `SplitComponent` class.

<a name="2.0.0-beta.4"></a>

# 2.0.0-beta.4 (2018-11-28)

- **Specific gutter style:** Add `<div>` inside `<div class="as-split-gutter">` to allow more customization.
- **Add SplitAreaDirective attribute selector:** You can now use `<as-split-area>` or `<div as-split-area>`, a class `as-split-area` is added to each areas for CSS targeting purpose.

<a name="2.0.0-beta.3"></a>

# 2.0.0-beta.3 (2018-11-26)

- **Style:** Modify `<as-split-area>` CSS selector to act only on current split areas children and not on potential sub split areas.

<a name="2.0.0-beta.2"></a>

# 2.0.0-beta.2 (2018-11-19)

- **Performance:** Make `@Output()` event emitters (`dragStart`, `dragProgress`, `dragEnd`, `gutterClick`, `transitionEnd`) works "lazily" to avoid useless change detection runs, especially for `dragProgress` which could be costly in big app.

<a name="2.0.0-beta.1"></a>

# 2.0.0-beta.1 (2018-11-17)

- **Styles:** Refactor the way styles are manage, no more `renderer.setStyle()` everywhere (except for areas `order` & `flex-basis`), now works with added/removed classes (`is-horizontal`/`is-vertical`, `is-disabled`, `is-transition`, `is-disabled`, `is-dragging`), way better. Doing like this, `<as-split-gutter>` directive is not needed anymore.

<a name="1.0.4"></a>

# 1.0.4 (2018-11-15)

- **Bug:** Fix Edge first rendering issue with nested split by applying css flex-direction property differently on `<as-split>` [#125](https://github.com/angular-split/angular-split/issues/125).

<a name="1.0.3"></a>

# 1.0.3 (2018-11-14)

- **Critiqual bug:** Remove reference to `TouchEvent` which cause error on Firefox & IE/Edge. Introduced in `1.0.1` but was there [before](https://github.com/angular-split/angular-split/blob/c71b7cf10a66a698820e91962d06cf35b726edc2/projects/angular-split/src/lib/component/split.component.ts#L478) on mobile browser other than chromium based.

<a name="1.0.2"></a>

# 1.0.2 (2018-11-13)

- **Bug:** Modify the way to emit gutterClick event which was buggy [#109](https://github.com/angular-split/angular-split/issues/109).

<a name="1.0.1"></a>

# 1.0.1 (2018-11-13)

- **Bug:** Some events were emitted outside of Zone.js leading to errors like [#118](https://github.com/angular-split/angular-split/issues/118) & [#109](https://github.com/angular-split/angular-split/issues/109).

<a name="1.0.0"></a>

# 1.0.0 (2018-11-10)

- **Project organization:** Now follow `@angular/cli` library management way which is awesome: [Library status update 📢](https://github.com/angular-split/angular-split/issues/122).
- **Dependencies:** `angular@^7` and `rxjs@^6` with pipe method (`rxjs-compat` not needed anymore).
- **Breaking changes:** Prefix `as-` added to component/directive to follow best practises: `<as-split>` & `<as-split-area>`.
- **Regression:** Revert change about `devicePixelRatio` added in `1.0.0-rc.3` because it was causing bad behavior on mobile [#85](https://github.com/angular-split/angular-split/issues/85), need to investigate more to resolve [#81](https://github.com/angular-split/angular-split/issues/81).

<a name="1.0.0-rc.3"></a>

# 1.0.0-rc.3 (2018-01-31)

- **Bug:** Use `devicePixelRatio` to make dragging value effective on HiDPI screen and browsers with zoom !== 100%, thanks to [tkglaser](https://github.com/tkglaser) and [HondaHiroyuki](https://github.com/HondaHiroyuki).

<a name="1.0.0-rc.1"></a>

# 1.0.0-rc.1 (2018-01-13)

- **Performances:** Put all event listeners inside `ngZone.runOutsideAngular()` to avoid triggering change detection during drag, thanks to [klemenoslaj](https://github.com/klemenoslaj).

<a name="1.0.0-rc.0"></a>

# 1.0.0-rc.0 (2017-12-01)

- **Bug:** Call `cdRef.markForCheck()` in several setters inside `SplitComponent` to force repaint if modified from TS class (instead of the template).

<a name="1.0.0-beta.9"></a>

# 1.0.0-beta.9 (2017-11-19)

- **Feature:** Add RTL support. Previously on 'right to the left' pages, dragging went opposite side, [issue here](https://github.com/angular-split/angular-split/issues/48). Now just add `dir="ltr"` on `<split>` component and that's fix.
- **Bug:** Fix small bug when updating `[gutterSize]` with `useTransition="true"`, now gutter's size got transition too and it's visually better.

<a name="1.0.0-beta.8"></a>

# 1.0.0-beta.8 (2017-11-17)

- **Bug:** When updating `[disabled]`, `[direction]`, `[width]`, `[height]`,.. keep size values got after gutter being dragged instead of reset to user provided values.
- **Bug:** When `[useTransition]="true"`, no more transition at component initialisation.

<a name="1.0.0-beta.7"></a>

# 1.0.0-beta.7 (2017-11-16)

- **gutterSize:** Default value from `10` to `11` because of a small discrepancy in the shown dots position pointed [there](https://github.com/angular-split/angular-split/issues/46).
- **Custom gutters style:** You can now use properties `[gutterColor]="'#ff0000'"`, `[gutterImageH]="'url(xxx)'"` and `[gutterImageV]="'url(xxx)'"`.

<a name="1.0.0-beta.6"></a>

# 1.0.0-beta.6 (2017-11-16)

- **Feature:** Emit `(gutterClick)` event even if `[disabled]="true"` to specific usecase.
- **Bug:** Fix bug occuring on split with `direction="vertical"` initialization, container height was wrong because `HostBinding` wasn't applied yet.

<a name="1.0.0-beta.5"></a>

# 1.0.0-beta.5 (2017-11-15)

- **Renaming:** `[visibleTransition]` property renamed to `[useTransition]` and work with `[visible]` & `[size]`.
- **Renaming:** `(visibleTransitionEnd)` event renamed to `(transitionEnd)` and now triggered from `[visible]` & `[size]` property.

<a name="0.2.7"></a>

# 0.2.7 (2017-11-14)

- **SemVer compatibility:** Copy of `0.2.3` to avoid breaking semantic versionning (I screwed up with `0.2.5` & `0.2.6` which needed angular >=5). Apps using angular 4.x having `"angular-split": "^0.2.2"` inside their `package.json` shoudn't break anymore.

<a name="1.0.0-beta.4"></a>

# 1.0.0-beta.4 (2017-11-13)

- **Bug:** Code rewrite to calculate new `flex-basis` values to avoid unwanted size flickering on areas not linked to dragged gutter.
- **Comment:** Add an explanation comment on `split.component.ts` top.

<a name="1.0.0-beta.3"></a>

# 1.0.0-beta.3 (2017-11-12)

- **Feature:** Accept number & boolean params as string to allow template syntax like `<split gutterSize="12" disabled="true">...</split>` or `<split-area order="4" size="40" visible="true">...</split-area>`.
- **Feature:** Add a `(gutterClick)` event for usecases like toggling area between 0% & X%. Now all drag events and gutterSize return `{gutterNum: number, sizes: Array<number>}`.

<a name="1.0.0-beta.2"></a>

# 1.0.0-beta.2 (2017-11-11)

- **Bug:** Fix bug when dragging gutter with previous area with `[visible]="false"` (bug there since the `[visible]` feature was added.. :( ).
- **Component access from JS/TS class:** You can now access `SplitComponent` and `SplitAreaDirective` as `ViewChild`/`ViewChildren` directly from your class to interact with.

<a name="1.0.0-beta.1"></a>

# 1.0.0-beta.1 (2017-11-10)

### Complete refactor, more robust, will be used as new base to add frequently asked features like `[minSize]` (pixel or percent) and custom style.

- **Allow area size init or drag to zero:** Refactor way to calcul area size `flex-basis: calc( X% - Ypx );` (seems easy at first sight but a bit painfull to implement). For example, you can now have 4 areas (with `[visible]="true"`), so 3 gutters, with sizes [0,0,0,100]. This was impossible before (size couldn't go down to 5%).
- **No more css `/deep/` use:** Could have used `::ng-deep` but I prefer to avoid it too.
- **Renderer2:** Use `Renderer2` instead of `Renderer` which is deprecated.

<a name="0.2.6"></a>

# 0.2.6 (2017-11-07)

- **UMD module fix:** Rollup config file wasn't correct.

<a name="0.2.5"></a>

# 0.2.5 (2017-11-06)

### Warning: Angular 5.0.0 minimum.

- **New files organisation:** Complete reorganisation of the github repository and files published on npm forked from this [library starter](https://github.com/robisim74/angular-library-starter).
- **New bundles generation:** Now you have umd bundles, flat ES module, and ES2015 flat ESM format.
- **Add tests:** This is what motivated me to change organisation, I will add others one soon `npm test`.

<a name="0.2.3"></a>

# 0.2.3 (2017-11-02)

- **Update package.json:** Moves dependencies to peerDependencies to be compatible with angular 5.x [pr59](https://github.com/angular-split/angular-split/pull/59).

<a name="0.2.2"></a>

# 0.2.2 (2017-08-04)

- **UMD bundle:** Add UMD bundle export thanks to [BenjaminDobler](https://github.com/BenjaminDobler).

<a name="0.2.1"></a>

# 0.2.1 (2017-07-18)

- **license:** Add an Apache license.
- **dependencies:** Update `rxjs` version inside `package.json`.

<a name="0.2.0"></a>

# 0.2.0 (2017-03-30)

- **ng upgrade:** upgrade to angular `^4.0.0`, replace `<template>` by `<ng-template>` and rebuild dist folder.

<a name="0.1.20"></a>

# 0.1.20 (2017-03-11)

- **wording:** add mention about CSS flexbox layout use, so `angular-split` is not compatible on browser not supporting it (like ios8).

### Feature

- **visibility toggle transition:** add transition (optionnal: `<split [visibleTransition]="true">`) when toggling visibility and `visibleTransitionEnd` event ` [pr11](https://github.com/angular-split/angular-split/pull/11).

<a name="0.1.19"></a>

# 0.1.19 (2017-02-09)

### Bug fix

- **gutter height on Safari:** fix a weird bug about anormal gutter height when direction is 'vertical' on Safari only [issue5](https://github.com/angular-split/angular-split/issues/5). Note that `angular-split` isn't working on browser without flexbox support, so not working on ios older than 9.

<a name="0.1.18"></a>

# 0.1.18 (2017-02-04)

### Bug fix

- **visibility toggle:** fix a bug I introduced in 0.1.17 while merging [pr10](https://github.com/angular-split/angular-split/pull/10).

<a name="0.1.17"></a>

# 0.1.17 (2017-02-03)

### Feature

- **visibility toggle:** add possibility to show/hide areas using `<split-area [visible]="boolean">` without removing them from the DOM, useful for specific case [like with router](https://github.com/jitsmaster/angular-split/commit/c7c92b9a1d1c00623660aeb7bc048509255e763b). Thanks to [jitsmaster](https://github.com/jitsmaster) ([pr8](https://github.com/angular-split/angular-split/pull/8) / [pr10](https://github.com/angular-split/angular-split/pull/10))
