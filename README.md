![libreact logo](./docs/assets/libreact.png)

# libreact

[![][npm-badge]][npm-url] [![][travis-badge]][travis-url] [![React Universal Interface](https://img.shields.io/badge/React-Universal%20Interface-green.svg)](https://github.com/streamich/react-universal-interface)

React standard library &mdash; must-have toolbox for any React project.

  - [React router](https://mailonline.github.io/libreact/en/routing.html), [sensors](https://mailonline.github.io/libreact/en/Sensors.html), [inversions](https://mailonline.github.io/libreact/en/Inversion.html), [context providers](https://mailonline.github.io/libreact/en/Context.html), [dummies](https://mailonline.github.io/libreact/en/Dummies.html), and [other goodies](https://mailonline.github.io/libreact/en/).
  - *Isomorphic* - all components work in browser and on server (and some in `react-native`).
  - See [__demos__](https://mailonline.github.io/libreact/demos/), [__docs__](https://mailonline.github.io/libreact/en/), and [__package__](https://www.npmjs.com/package/libreact/).


## Installation

<pre>
npm i <a href="https://www.npmjs.com/package/libreact">libreact</a> --save
</pre>


## Usage

Import each utility individually to decrease your bundle size

```js
import {mock} from 'libreact/lib/mock';

const MyComponent = mock();
```


## Contents

  - [Introduction](./docs/en/Introduction.md)
  - [Dummies](./docs/en/Dummies.md)
     - [`mock()`](./docs/en/mock.md) and [`loadable()`](./docs/en/loadable.md) &mdash; [**example**](https://codesandbox.io/s/j2ovpr03z3)
     - [`lazy()`](./docs/en/lazy.md), [`delayed()`](./docs/en/delayed.md), and [`viewport()`](./docs/en/viewport.md)
  - [Inversion](./docs/en/Inversion.md)
     - [`<State>`](./docs/en/State.md) and [`withState()`](./docs/en/State.md#withstate-hoc)
        - [`<Toggle>`](./docs/en/Toggle.md), [`withToggle()`](./docs/en/Toggle.md#withtoggle-hoc), and [`@withToggle`](./docs/en/Toggle.md#withtoggle-decorator) &mdash; [**example**](https://codesandbox.io/s/zwkl16vv93)
        - [`<Flipflop>`](./docs/en/Flipflop.md), [`withFlipflop()`](./docs/en/Flipflop.md#withflipflop-hoc), and [`@withFlipflop`](./docs/en/Flipflop.md#withflipflop-decorator)
        - [`<Value>`](./docs/en/Value.md), [`withValue()`](./docs/en/Value.md#withvalue-hoc), and [`@withValue`](./docs/en/Value.md#withvalue-decorator)
        - [`<Counter>`](./docs/en/Counter.md), [`withCounter()`](./docs/en/Counter.md#withcounter-hoc) and [`@withCounter`](./docs/en/Counter.md#withcounter-decorator)
        - [`<List>`](./docs/en/List.md), [`withList()`](./docs/en/List.md#withlist-hoc), and [`@withList`](./docs/en/List.md#withlist-decorator)
        - [`<Map>`](./docs/en/Map.md), [`withMap()`](./docs/en/Map.md#withmap-hoc), and [`@withMap`](./docs/en/Map.md#withmap-decorator)
     - [`<ShouldUpdate>`](./docs/en/ShouldUpdate.md), [`shouldUpdate()`](./docs/en/ShouldUpdate.md#shouldupdate-hoc), and [`pure()`](./docs/en/pure.md)
     - [`<Lifecycles>`](./docs/en/Lifecycles.md)
     - [`invert()`](./docs/en/invert.md) and [`<Inverted>`](./docs/en/invert.md#inverted)
  - [Sensors](./docs/en/Sensors.md)
     - [`<ActiveSensor>`](./docs/en/ActiveSensor.md), [`withActive()`](./docs/en/ActiveSensor.md#withactive-hoc), and [`@withActive`](./docs/en/ActiveSensor.md#withactive-decorator)
     - [`<BatterySensor>`](./docs/en/BatterySensor.md), [`withBattery()`](./docs/en/BatterySensor.md#withbattery), and [`@withBattery`](./docs/en/BatterySensor.md#withbattery-1)
     - [`<ExitSensor>`](./docs/en/ExitSensor.md) &mdash; [**example**](https://codesandbox.io/s/7437x10z71)
     - [`<FocusSensor>`](./docs/en/FocusSensor.md), [`withFocus()`](./docs/en/FocusSensor.md#withfocus-hoc), and [`@withFocus`](./docs/en/FocusSensor.md#withfocus-decorator)
     - [`<GeoLocationSensor>`](./docs/en/GeoLocationSensor.md), [`withGeoLocation()`](./docs/en/GeoLocationSensor.md#withgeolocation-hoc), and [`@withGeoLocation`](./docs/en/GeoLocationSensor.md#withgeolocation-decorator)
     - [`<HoverSensor>`](./docs/en/HoverSensor.md), [`withHover()`](./docs/en/HoverSensor.md#withhover-hoc), and [`@withHover`](./docs/en/HoverSensor.md#withhover-decorator) &mdash; [**example**](https://codesandbox.io/s/8p3xqx83p9)
     - [`<IdleSensor>`](./docs/en/IdleSensor.md), [`withIdle()`](./docs/en/IdleSensor.md#withidle-hoc), and [`@withIdle`](./docs/en/IdleSensor.md#withidle-decorator)
     - [`<MediaDeviceSensor>`](./docs/en/MediaDeviceSensor.md), [`withMediaDevices()`](./docs/en/MediaDeviceSensor.md#withmediadevices), and [`@withMediaDevices`](./docs/en/MediaDeviceSensor.md#withmediadevices-1)
     - [`<MediaSensor>`](./docs/en/MediaSensor.md), [`withMedia()`](./docs/en/MediaSensor.md#withmedia), and [`@withMedia`](./docs/en/MediaSensor.md#withmedia-1)
     - [`<MotionSensor>`](./docs/en/MotionSensor.md), [`withMotion()`](./docs/en/MotionSensor.md#withmotion-hoc), and [`@withMotion`](./docs/en/MotionSensor.md#withmotion-decorator)
     - [`<MouseSensor>`](./docs/en/MouseSensor.md), [`withMouse()`](./docs/en/MouseSensor.md#withmouse-hoc), and [`@withMouse`](./docs/en/MouseSensor.md#withmouse-decorator) &mdash; [**example**](https://codesandbox.io/s/k3o16j7n47)
     - [`<NetworkSensor>`](./docs/en/NetworkSensor.md), [`withNetwork()`](./docs/en/NetworkSensor.md#withnetwork-hoc), and [`@withNetwork`](./docs/en/NetworkSensor.md#withnetwork-decorator)
     - [`<LightSensor>`](./docs/en/LightSensor.md), [`withLight()`](./docs/en/LightSensor.md#withlight-hoc), and [`@withLight`](./docs/en/LightSensor.md#withlight-decorator)
     - [`<LocationSensor>`](./docs/en/LocationSensor.md), [`withLocation()`](./docs/en/LocationSensor.md#withlocation-hoc), and [`@withLocation`](./docs/en/LocationSensor.md#withlocation-decora)
     - [`<OrientationSensor>`](./docs/en/OrientationSensor.md), [`withOrientation()`](./docs/en/OrientationSensor.md#withorientation-hoc), and [`@withOrientation`](./docs/en/OrientationSensor.md#withorientation-decorator)
     - [`<ScratchSensor>`](./docs/en/ScratchSensor.md), [`withScratch()`](./docs/en/ScratchSensor.md#withscratch-hoc), and [`@withScratch`](./docs/en/ScratchSensor.md#withscratch-decorator)
     - [`<ScrollSensor>`](./docs/en/ScrollSensor.md)
     - [`<SizeSensor>`](./docs/en/SizeSensor.md), [`withSize()`](./docs/en/SizeSensor.md#withsize-hoc), and [`@withSize`](./docs/en/SizeSensor.md#withsize-decorator) &mdash; [**example**](https://codesandbox.io/s/0y2qjm210p)
        - [`<WidthSensor>`](./docs/en/WidthSensor.md), [`withWidth()`](./docs/en/WidthSensor.md#withwidth-hoc-and-withwidth-decorator), and [`@withWidth`](./docs/en/WidthSensor.md#withwidth-hoc-and-withwidth-decorator)
     - [`<ViewportSensor>`](./docs/en/ViewportSensor.md), [`withViewport()`](./docs/en/ViewportSensor.md#withviewport-hoc), and [`@withViewport`](./docs/en/ViewportSensor.md#withviewport-decorator)
        - [`<ViewportScrollSensor>`](./docs/en/ViewportSensor.md#viewportscrollsensor) and [`<ViewportObserverSensor>`](./docs/en/ViewportSensor.md#viewportobserversensor)
     - [`<WindowScrollSensor>`](./docs/en/WindowScrollSensor.md), [`withWindowScroll()`](./docs/en/WindowScrollSensor.md#withwindowscroll-hoc), and [`@withWindowScroll`](./docs/en/WindowScrollSensor.md#withwindowscroll-decorator)
     - [`<WindowSizeSensor>`](./docs/en/WindowSizeSensor.md), [`withWindowSize()`](./docs/en/WindowSizeSensor.md#withwindowsize-hoc), and [`@withWindowSize`](./docs/en/WindowSizeSensor.md#withwindowsize-decorator)
  - [Context](./docs/en/Context.md)
     - [`<Provider>`](./docs/en/Provider.md#provider), [`<Consumer>`](./docs/en/Provider.md#consumer), [`withContext()`](./docs/en/Provider.md#withcontext-hoc), and [`@withContext`](./docs/en/Provider.md#withcontext-decorator)
     - [`<Theme>`](./docs/en/theme.md#theme), [`<Themed>`](./docs/en/theme.md#themed), [`withTheme()`](./docs/en/theme.md#withtheme-hoc), and [`@withTheme`](./docs/en/theme.md#withtheme-decorator)
     - [`<CssVarsProvider>`](./docs/en/cssvars.md), [`<CssVars>`](./docs/en/cssvars.md#cssvars), [`withCssVars()`](./docs/en/cssvars.md#withcssvars-hoc), and [`@withCssVars`](./docs/en/cssvars.md#withcssvars-decorator)
     - [`<Router>`](./docs/en/routing.md#router), [`<Route>`](./docs/en/routing.md#route), [`withRoute()`](./docs/en/routing.md#withroute), `@withRoute`, `go()`, and `<Go>`
     - [`<Translations>`](./docs/en/translate.md#translations), [`<Translate>`](./docs/en/translate.md#translate-or-t), [`<T>`](./docs/en/translate.md#translate-or-t), [`withT()`](./docs/en/translate.md#witht-hoc), and [`@withT`](./docs/en/translate.md#witht-decorator)
  - [UI](./docs/en/UI.md)
     - [`<Portal>`](./docs/en/Portal.md), [`<Overlay>`](./docs/en/Overlay.md), and [`<Modal>`](./docs/en/Modal.md)
     - [`<Dimmer>`](./docs/en/Dimmer.md) and [`<Dimmable>`](./docs/en/Dimmable.md)
     - [`<FullScreen>`](./docs/en/FullScreen.md)
     - [`<Slider>`](./docs/en/Slider.md)
     - [`<DropArea>`](./docs/en/DropArea.md)
     - [`<Group>`](./docs/en/Group.md)
     - [`<OutsideClick>`](./docs/en/OutsideClick.md)
     - [`<Ripple>`](./docs/en/Ripple.md) and [`withRipple()`](./docs/en/Ripple.md#withripple) &mdash; [**example**](https://codesandbox.io/s/983q7jr80o)
     - [`<Img>`](./docs/en/Img.md)
     - [`<WidthQuery>`](./docs/en/WidthQuery.md), [`<View>`](./docs/en/View.md), [`<WindowWidthQuery>`](./docs/en/WindowWidthQuery.md), and [`<InlineWidthQuery>`](./docs/en/InlineWidthQuery.md)
     - [`<Audio>`](./docs/en/Audio.md) and [`<Video>`](./docs/en/Video.md)
     - [`<Speak>`](./docs/en/Speak.md), [`<Vibrate>`](./docs/en/Vibrate.md), [`<Alert>`](./docs/en/Alert.md), `<Prompt>`, `<Confirm>`
  - [Animation](./docs/en/Animation.md)
     - [`<AfterTimeout>`](./docs/en/AfterTimeout.md), [`<AfterDraf>`](./docs/en/AfterDraf.md), and [`<WhenIdle>`](./docs/en/WhenIdle.md)
     - [`<Render>`](./docs/en/Render.md), [`withRender()`](./docs/en/Render.md#withrender-hoc), and [`@withRender`](./docs/en/Render.md#withrender-decorator)
     - [`<RenderInterval>`](./docs/en/RenderInterval.md), [`withRenderInterval()`](./docs/en/RenderInterval.md#withrenderinterval-hoc), and [`@withRenderInterval`](./docs/en/RenderInterval.md#withrenderinterval-decorator)
     - [`<Tween>`](./docs/en/Tween.md), [`withTween()`](./docs/en/Tween.md#withtween-hoc), and [`@withTween`](./docs/en/Tween.md#withtween-decorator)
     - [`<Interpolation>`](./docs/en/Interpolation.md), [`withInterpolation()`](./docs/en/Interpolation.md#withinterpolation-hoc), and [`@withInterpolation`](./docs/en/Interpolation.md#withinterpolation-decorator)
  - [Side Effects](./docs/en/Side-effects.md)
     - [`<LocalStorage>`](./docs/en/LocalStorage.md), `<SessionStorage>`, `<IndexedDb>`
     - [`<ClassNames>`](./docs/en/ClassNames.md)
     - `<Title>`, `<Favicon>`
     - [`go()`](./docs/en/routing.md#go), `<Redirect>`, `<Link>`, [`<Sms>`](./docs/en/Sms.md), [`<Mailto>`](./docs/en/Mailto.md), and `<Tel>`
  - [Boundaries](./docs/en/Boundaries.md)
     - [`<BrowserOnly>`](./docs/en/BrowserOnly.md), [`<ServerOnly>`](./docs/en/ServerOnly.md), and [`<ElectronOnly>`](./docs/en/ElectronOnly.md)
     - [`<ErrorBoundary>`](./docs/en/ErrorBoundary.md) and [`withErrorBoundary()`](./docs/en/ErrorBoundary.md#witherrorboundary-hoc)
     - `<CacheBoundary>`
  - [NEXT](./docs/en/next.md)
     - [`createRef()`](./docs/en/next/createRef.md), [`createState()`](./docs/en/next/createState.md), and [`createLifecycleEvents()`](./docs/en/next/createLifecycleEvents.md)
  - Other
     - [`<Resolve>`](./docs/en/Resolve.md), `<Fetch>`
     - [`getDisplayName()`](./docs/en/getDisplayName.md)
     - `<Locales>`
     - `<Draggable>`, `<Droppable>`, `<Parallax>`, `<Pin>`
  - Electron
     - `<Menu>` and `<MenuItem>`


## License

[Unlicense](./LICENSE) &mdash; public domain.


[npm-url]: https://www.npmjs.com/package/libreact
[npm-badge]: https://img.shields.io/npm/v/libreact.svg
[travis-url]: https://travis-ci.org/MailOnline/libreact
[travis-badge]: https://travis-ci.org/MailOnline/libreact.svg?branch=master
