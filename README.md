### Tom

First-year at the University of Nebraska Omaha. I build infrastructure for running many AI coding
agents at once, and native macOS tools.

| | |
|---|---|
| [**overseer**](https://github.com/tomarai85/overseer) | A local cockpit for a fleet of AI coding agents. The hard part is not the dashboard — it is deciding, from a transcript and a pid, whether a session is *working*, *blocked*, *waiting on you*, or *safe to restart*. Get that wrong and you either restart an agent mid-edit or leave it hung for an hour. 3.6k lines of Python, 17 test files, and a written market read that names its own weakest moat. |
| [**dualsense-bridge**](https://github.com/tomarai85/dualsense-bridge) | The PS5 DualSense's built-in mic, as a real macOS microphone, over Bluetooth, with no extra hardware. Sony's docs, macOS, and the standard libraries all treat that mic as USB-only; the projects that do capture it wirelessly need a Raspberry Pi Pico dongle. The audio turns out to be Opus-encoded inside the controller's HID input reports — decode it on the host, hand it to a virtual CoreAudio device, and "DualSense Mic" shows up in System Settings like any other input. |
| [**court-recover**](https://github.com/tomarai85/court-recover) | 95 lines of bash that catch one specific way an AI agent fails — it *writes* a tool call as prose instead of *making* it, then waits forever — and force a clean retry. Fail-open: if the hook itself breaks, the session continues. CI on every push. |
| [**Flote**](https://github.com/tomarai85/flote) | Shipped macOS app with a [site](https://flote-app.vercel.app) and install steps. Option+Space floats a sticky note; write the thought as it comes out, press Organize once, and it becomes a title, key points and a checklist. |

Work in other people's repositories: a multi-account switching change **merged into**
[steipete/CodexBar](https://github.com/steipete/CodexBar), and a multi-display window fix plus a
battery-floor safety **sent to** [fuji-mak/Capsomnia](https://github.com/fuji-mak/Capsomnia) (open).
**claudebar** is my build of CodexBar — the app is his, the multi-account switching is mine.
