# Why this repo

After an X.org Linux install, I always have to remember which flags I need to change in Firefox, in order to match my personal configuration.

**I made this repo so I will not misconfigure the browser in the future.**

## Hardware acceleration
- `layers.acceleration.force-enabled`: `true`
- `gfx.webrender.all`: `true`

## Hardware video decoding
_You need a working VAAPI configuration for this. Also, set_ `MOZ_X11_EGL=1` _env variable._

- `media.ffmpeg.vaapi.enabled`: `true`
- `media.ffvpx.enabled`: `false`
- `media.rdd-vpx.enabled`: `false`
- `media.navigator.mediadatadecoder_vpx_enabled`: `true`
- `media.av1.enabled`: `false`

## Disable autohide in fullscreen
- `browser.fullscreen.autohide`: `false`

## Sensible full screen
- `full-screen-api.transition-duration.enter`: `0 0`
- `full-screen-api.transition-duration.leave`: `0 0`
- `full-screen-api.transition.timeout`: `0`
- `full-screen-api.warning.delay`: `0`
- `full-screen-api.warning.timeout`: `0`

## Context menus on mouse up (WM)
- `ui.context_menus.after_mouseup`: `true`

## Touchpad scroll
- `apz.gtk.kinetic_scroll.enabled`: `false`

