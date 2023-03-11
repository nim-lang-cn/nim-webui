# WebUI

> Use any web browser as GUI, with Nim in the backend, and
> HTML/Nim/JS/TS/CSS in the frontend.

Nim wrapper and bindings for WebUI, a fully independent cross-platform web UI
library.

Instead of using a third-party library, WebUI instead uses a pre-installed
browser (Edge, Firefox, Chrome, Chromium, or Safari). So, there's no need for any
large SDK or library for development/production, all you need is a web browser!

> :warning: **Notice**:
>
> * WebUI is not a web-server solution or a framework, but it's an easy-embeddable
> tool to use any installed web browser as a user interface.
>
> * Documentation is **not** finished.
>
> * WebUI is not ready yet for production release.

## Features

- Fully Independent (*No need for any third-party library*)
- Lightweight (*~600 Kb* (*300 Kb when compiling with DLL*)) & Small memory footprint
- Fast WS binary communication (*App--WebUI--Browser*)
- One Nim file
- Multi-platform & Multi-Browser
- Using private profile for safety

## Installation

Install via Nimble:

```shell
nimble install https://github.com/neroist/webui
```

## Documentation

Online documentation can be found here: <https://neroist.github.io/webui>

There isn't much documentation as of right now, so I suggest to get started
using the examples at [`examples/`](examples/).

Heres a very [*minimal*](examples/minimal.nim) example of using the wrapper:

```nim
import webui

let window = newWindow() # Create a new Window
window.show("<html>Hello</html>") # Show the window with html content

wait() # Wait until the window gets closed
```

## Supported Browsers

| OS      | Browser | Status        |
| ------  | ------  | ------        |
| Windows | Firefox | ✔️            |
| Windows | Chrome  | ✔️            |
| Windows | Edge    | ✔️            |
| Linux   | Firefox | ✔️            |
| Linux   | Chrome  | ✔️            |
| macOS   | Firefox | *coming soon* |
| macOS   | Chrome  | *coming soon* |
| macOS   | Safari  | *coming soon* |

## License

MIT License. See [LICENSE](LICENSE)

Original WebUI library is licensed under GPL-3.0. See
[LICENSE](https://github.com/alifcommunity/webui/blob/main/LICENSE).
