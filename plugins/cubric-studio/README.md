# Cubric Studio

Let Claude make images, video and GIFs in [Cubric Studio](https://cubric.studio), the desktop
app on your computer. Ask for "an image of a red bicycle in a new project" and it lands in your
gallery as a real card, with its prompt and settings saved, ready to edit by hand.

You need **Cubric Studio 2.0 or newer**, installed and **open** on the same computer as Claude.

It works in **Claude Code** (the terminal, or the Code tab of the Claude desktop app) and in
Codex. In Claude chat, on the web, in the desktop app or on a phone, the plugin loads without its
tools, so Claude cannot reach the app from there. For chat in the Claude desktop app, add the
Cubric Studio extension:
[install steps](https://github.com/MadPonyInteractive/cubric-studio-agents#install).

## What it does

The plugin gives Claude the app's own tools: list models and read their prompting guides, create
and open projects, generate and edit images and video (with your own files as references), run
Flows, look at the results, rename cards, and make and edit GIFs.

- **Paid cloud models ask first.** Claude is told the price and must confirm it with you before
  anything is billed. Local models are free and never ask.
- **Nothing deletes.** No tool removes a project, a card or a file, and none installs a model.

## What it runs and connects to

One small MCP server, `server/index.js`, started with `node` (Node.js 18 or newer must be
installed). It is a bridge with no dependencies: it passes each message from Claude to the
Cubric Studio app on your own computer, at `http://127.0.0.1:24300/mcp` (or `127.0.0.1:3000`
for an app older than 2.2.3), and passes the app's answer back. When the app is closed it says
so and offers one `status` tool until the app opens. The bridge downloads nothing and connects
to no other address. A skill tells Claude how to use the tools.

## Privacy Policy

This plugin collects no data and sends nothing anywhere except to the Cubric Studio app on your
own computer. It keeps no data of its own, so there is nothing to retain or delete. Your agent's
provider sees what your agent sees, including the pictures it looks at, under that provider's
own terms. What the Cubric Studio app itself collects and stores, which services it shares data
with, and how long anything is kept are set out in the app's privacy policy:
[cubric.studio/privacy](https://cubric.studio/privacy/).

## Contact

contact@madponyinteractive.com
