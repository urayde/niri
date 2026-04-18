<h1 align="center"><img alt="niri" src="https://github.com/user-attachments/assets/ec419528-b1f7-4041-b1be-ecf9865f0be7"></h1>
<p align="center">A scrollable-tearing Wayland compositor.</p>

## About

This fork features basic support for screen tearing (along with some other niceties), and likely will exist until upstream does. If you're having issues in games with input latency from VSync - give it a shot!

To get this running on your system, you will need to follow [build instructions](https://github.com/urayde/niri/blob/main/docs/wiki/Getting-Started.md#building).
For Arch-based distributions, you can install it via [AUR](https://aur.archlinux.org/packages/niri-tearing-git).

To enable screen tearing, use a [debug option](https://github.com/urayde/niri/blob/main/docs/wiki/Configuration%3A-Debug-Options.md#force-tearing) or a [window rule](https://github.com/urayde/niri/blob/main/docs/wiki/Configuration%3A-Window-Rules.md#allow-tearing). Some applications (such as GE-Proton) may request tearing automatically.

## Features

- [Explicit sync](https://wayland.app/protocols/linux-drm-syncobj-v1) (could be disabled with `NIRI_DISABLE_SYNCOBJ=1`)
- [Tearing control](https://wayland.app/protocols/tearing-control-v1)
- [FIFO constraints](https://wayland.app/protocols/fifo-v1)
- [Pointer warp](https://wayland.app/protocols/pointer-warp-v1) (upstream PR [#4001](https://github.com/niri-wm/niri/pull/4001))
