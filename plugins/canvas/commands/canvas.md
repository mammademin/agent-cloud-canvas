---
description: Put this project's app on your canvas, beside the chat
argument-hint: [port]
---
Put my app on my canvas, beside this chat, with the canvas tools (this plugin's show_local).

If I wrote a port after /canvas, use http://localhost:<that port>/ and skip finding: $ARGUMENTS
Find the app yourself, without asking me:
1. This project's app, if it's running: list the ports this machine listens on with their processes (macOS and Linux: lsof -nP -iTCP -sTCP:LISTEN), and keep those whose process works in this project's folder (lsof -a -p <pid> -d cwd). Of those, prefer one whose / answers a web page, and the one started most recently.
2. If none is running, start this project's dev command in the background (the dev or start script in package.json, or the framework's own), and use the address it prints.
3. Ask me only if there's no app to find or start.
Then call show_local with that address and a short name (the project's), start the helper (and the door, for your own browser) as its answer says, and open the canvas beside this chat. Tell me in one line which app you put there, so I can say "/canvas <port>" for another. Don't mention helpers, ports or sign-in otherwise.
