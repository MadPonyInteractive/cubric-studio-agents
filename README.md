# Cubric Studio for AI agents

Let your AI agent make images, video and GIFs in [Cubric Studio](https://cubric.studio), the
desktop app on your computer. Ask Claude, Codex or Antigravity for "an image of a red bicycle in
a new project" and it lands in your gallery as a real card, with its prompt and settings saved.

You need **Cubric Studio 2.0 or newer**, installed and **open**. Earlier versions have no agent
connection. Your agent reaches the app at `http://127.0.0.1:3000/mcp`, on your own computer only;
in Claude Code, the plugin's **Cubric Studio address** setting changes it if you started the app
on another port.

## Install

**The easy way**: in Cubric Studio, open **Settings > Connect an agent** and press **Connect**
next to your agent. The app runs the steps below for you. The manual steps work on Windows,
macOS and Linux.

**Claude Code**

```
/plugin marketplace add https://github.com/MadPonyInteractive/cubric-studio-agents.git
/plugin install cubric-studio@cubric-studio
```

Use the full `https://` address: the short `MadPonyInteractive/cubric-studio-agents` form clones
over SSH, which fails unless you have a GitHub SSH key set up.

**Codex**

```
codex plugin marketplace add MadPonyInteractive/cubric-studio-agents
codex plugin add cubric-studio@cubric-studio
```

**Claude Desktop** (Windows and macOS; there is no Claude Desktop for Linux): download
[cubric-studio.mcpb](https://github.com/MadPonyInteractive/cubric-studio-agents/releases/latest/download/cubric-studio.mcpb),
then in Claude Desktop open **Settings > Extensions** and drag the file onto that page. Claude
shows what it installs and asks you to confirm. Double-clicking the file only works where your
computer already opens `.mcpb` files with Claude.

**Antigravity**: download this repository (Code > Download ZIP), copy the
`plugins/cubric-studio` folder into `%USERPROFILE%\.gemini\config\plugins\` (on macOS and Linux,
`~/.gemini/config/plugins/`), then restart Antigravity.

**ChatGPT**: use Codex, which comes with your ChatGPT plan. The ChatGPT chat window runs in the
cloud and cannot reach apps on your computer.

**Gemini**: use Antigravity, Google's agent app for your computer (install steps above). It is
free to start with the Google account you use for Gemini, no subscription needed; a Google AI Pro
or Ultra plan gives it more use. The Gemini app and gemini.google.com run in the cloud and cannot
reach apps on your computer.

## What your agent can do

List models and read their prompting guides, create and open projects, generate and edit images
and video (with your own files as references), run Flows, look at the results, rename cards, and
make and edit GIFs.

- **Paid cloud models ask first.** The agent is told the price and must confirm it before
  anything is billed. Local models are free and never ask.
- **Nothing deletes.** No tool removes a project, a card or a file, and none installs a model.

## Privacy

This plugin connects your agent to the app on your own computer and nowhere else. Your agent's
provider (Anthropic, OpenAI or Google) sees what your agent sees, including the pictures it looks
at. What the app itself sends, and where, is listed at
[cubric.studio/privacy](https://cubric.studio/privacy/).

## Contact

contact@madponyinteractive.com
