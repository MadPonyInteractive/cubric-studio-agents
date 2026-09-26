# Cubric Studio for AI agents

Let your AI agent make images, video and GIFs in [Cubric Studio](https://cubric.studio), the
desktop app on your computer. Ask Claude, Codex or Antigravity for "an image of a red bicycle in
a new project" and it lands in your gallery as a real card, with its prompt and settings saved.

You need **Cubric Studio 1.7 or newer**, installed and **open**. Earlier versions have no agent
connection, so until 1.7 is released this plugin has nothing to talk to. Your agent reaches the
app at `http://127.0.0.1:3000/mcp`, on your own computer only.

## Install

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

**Claude Desktop**: download
[cubric-studio.mcpb](https://github.com/MadPonyInteractive/Cubric-Studio/releases/latest/download/cubric-studio.mcpb)
and double-click it.

**Antigravity**: download this repository (Code > Download ZIP), copy the
`plugins/cubric-studio` folder into `%USERPROFILE%\.gemini\config\plugins\` (on macOS and Linux,
`~/.gemini/config/plugins/`), then restart Antigravity.

**ChatGPT**: use Codex, which comes with your ChatGPT plan. The ChatGPT chat window runs in the
cloud and cannot reach apps on your computer.

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
