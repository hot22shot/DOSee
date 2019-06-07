# DOSee

## Changes and updates

### v1.20

- Now requires [npm](https://www.npmjs.com/get-npm) or [Docker](https://www.docker.com/products/docker-desktop) for installation as the installation scripts have been removed.
- Added `DOSee` prototype object that is accessible from `window.DOSee`. It is now used to access all the custom DOSee function additions.
- Added `DOSee.exit()` that will end the emulation and remove all event listeners created by Emscripten.
- Added `DOSee.canvasResize()` that uses Emscripten to resize the canvas element.
- Added `dosee:spacekeystart` meta element to disable the Space key to start DOSee feature.
- Removed the right-click menu over the canvas blocker that was used by The Emularity, there are a couple of screen capture items instead.
- Isolated the variables and functions in `dosee-init.js` so they do not pollute the `window` global scope.

### v1.13

- Now will read and use `<meta data="dosee:filename">` element.

### v1.11

- Added a PowerShell install script for Windows (and PowerShell Core) users.
- Replaced `doseeVersion` string with a `version` Map() object.
- Replaced the use of the outdated and broken _screenfull_ library with the [Fullscreen API](https://developer.mozilla.org/en-US/docs/Web/API/Fullscreen_API).
- Fixed missing dependencies false-positives.
- _doseeTabs_ links now anchor back to `<header id="doseeTabs">`

### v1.10

- Initial public release.