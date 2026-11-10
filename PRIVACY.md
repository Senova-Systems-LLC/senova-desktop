# Senova for Windows: privacy notice

Last updated: 10 November 2026

Senova Systems LLC ("Senova", "we") makes the Senova desktop app. This notice covers the desktop app
only. The website and Senova online have their own privacy policy at senovasys.com.

## The short version
- Senova's models run on your PC. Your chats, files, projects, artifacts and code stay on your PC.
- The desktop app sends nothing to Senova's servers. It has no analytics, no tracking and no usage reporting.
- Some features reach the internet when you use them, and only to the service that feature needs (listed below).
- You can export or delete all of your data in Settings > Privacy & data.

## What is stored on your PC
| Data | Where | How long |
| --- | --- | --- |
| Chats, projects, knowledge files, artifacts, memories, settings | `%USERPROFILE%\.senova` (a local database and files) | Until you delete them |
| Code sessions: checkpoints, diffs and command output | `%USERPROFILE%\.senova` and your project folders | Until you delete the session |
| Action log (what Senova did with screen control, apps and commands) | `%USERPROFILE%\.senova` | Until you clear it |
| Screenshots taken for screen control | In memory for the next step only. If you turn on "keep screenshots", they are saved, encrypted with your Windows account key (DPAPI), and deleted with the log | As above |
| App logs and crash reports | `%APPDATA%\Senova\logs` and `%APPDATA%\Senova\Crashpad`, on your PC only, never uploaded | The log is rotated at 5 MB (one older file is kept). Crash reports stay until you delete them |
| Setup answers (terms accepted and when, update setting) | `%APPDATA%\Senova\desktop.json` | Until you uninstall and delete it |
| Model files | `%USERPROFILE%\.senova\models` | Until you remove them |

## When the app goes online, and what it sends
| Feature | Goes to | What is sent | When |
| --- | --- | --- | --- |
| Model download | The model hosts listed in `models/sources.json` (for example Hugging Face and Ollama) | A normal download request (your IP address) | First run, and when you add a model |
| App updates | GitHub (github.com, where Senova releases are published) | A request for the latest version (your IP address and app version) | At start-up and every 6 hours. You can turn this off in the tray menu ("Check for updates automatically") |
| Web search | DuckDuckGo, or Brave Search if you add a Brave key | Your search query | Only when a chat uses web search |
| Imports | GitHub, YouTube, or the address you give | The address of what you import | Only when you import something |
| Artifacts | Public CDNs (cdnjs, jsDelivr, unpkg, esm.sh, Google Fonts) | Requests for libraries and fonts that an artifact uses | When an artifact needs one that isn't bundled |
| Connectors (MCP) and GitHub | The service you connect, through your own login (for example `gh`) | What that tool call needs. Every call asks you first | Only after you connect one |
| Senova in Chrome | Your own Chrome, through the extension | Pages you ask Senova to read or act on | Only when you use it |

Those services handle that data under their own privacy policies. Senova does not receive it.

## Screen control and app control
- Off until you turn it on, and then only for the apps you grant. Banking, password managers and Windows security tools can never be granted.
- While Senova controls the screen, a glowing border and a notice show it, and Esc or the kill switch stops it at once.
- Screenshots go only to the model running on your PC.

## Phone pairing
- The phone app pairs with a one-time code shown on your PC. The phone makes its own key pair, and every approval it sends is signed.
- In this version the phone reaches the desktop app only on the same computer. No relay server and no push notifications are used yet. If we add a relay, this notice will be updated first, and the relay will only carry encrypted, signed messages.
- The phone keeps its pairing key and a list of pending approvals. You can unpair from either side.

## Your choices
- Export or delete everything: Settings > Privacy & data.
- Turn off web search, screen control and connectors in Settings, and update checks in the tray menu.
- Uninstall: removes the app. Your chats and models in `%USERPROFILE%\.senova` stay, so a reinstall keeps them. Delete them first in Settings > Privacy & data, or delete that folder.

## Children
Senova is not meant for children under 13, or under 16 in the EU and UK.

## Contact
Senova Systems LLC, New Jersey, USA, hello@senovasys.com.
