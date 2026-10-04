# Cubric Studio

Let Claude make images, video and GIFs in [Cubric Studio](https://cubric.studio), the desktop
app on your computer. Ask for "an image of a red bicycle in a new project" and it lands in your
gallery as a real card, with its prompt and settings saved, ready to edit by hand.

You need **Cubric Studio 2.0 or newer**, installed and **open** on the same computer as Claude.

## What it does

The plugin gives Claude the app's own tools: list models and read their prompting guides, create
and open projects, generate and edit images and video (with your own files as references), run
Flows, look at the results, rename cards, and make and edit GIFs.

- **Paid cloud models ask first.** Claude is told the price and must confirm it with you before
  anything is billed. Local models are free and never ask.
- **Nothing deletes.** No tool removes a project, a card or a file, and none installs a model.

## What it runs and connects to

One MCP server, reached over HTTP at the address the Cubric Studio app listens on, on your own
computer: `http://127.0.0.1:3000/mcp` unless you change the **Cubric Studio address** setting
(only needed if you started the app on another port). The plugin runs no program of its own,
downloads nothing, and connects to no other address. A skill tells Claude how to use the tools.

## Privacy Policy

This plugin collects no data and sends nothing anywhere except to the Cubric Studio app on your
own computer. It keeps no data of its own, so there is nothing to retain or delete. Your agent's
provider sees what your agent sees, including the pictures it looks at, under that provider's
own terms. What the Cubric Studio app itself collects and stores, which services it shares data
with, and how long anything is kept are set out in the app's privacy policy:
[cubric.studio/privacy](https://cubric.studio/privacy/).

## Contact

contact@madponyinteractive.com
