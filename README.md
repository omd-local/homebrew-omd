# OMD Homebrew tap

Install the current public beta of OMD on macOS:

```bash
brew install omd-local/omd/omd
```

Then verify the command-line tools and backend capabilities:

```bash
omd --version
omd doctor
omd capabilities --json
omd-mcp < /dev/null
```

For the complete Mac workflow, install **OMD Home 0.2.2** in Obsidian and use
the matching **OMD backend 0.3.0b5** from this tap:

- [中文安装与首次使用指南](https://github.com/omd-local/obsidian-omd-home/blob/main/docs/getting-started-mac.md)
- [English installation and first-use guide](https://github.com/omd-local/obsidian-omd-home/blob/main/docs/getting-started-mac.en.md)

Existing users can run `brew update`, then `brew upgrade omd-local/omd/omd`.
The plugin and backend are updated separately. Speech transcription, Ollama
models, and the Calendar helper are optional, separate setup steps described
in the guides; basic capture does not need AI.

The browser UI remains deferred while its dependencies await a compatible
audited release. `omd-ui` explains its unavailability and does not start a
server. OMD Home, the CLI, and MCP do not require that browser UI.

Project documentation and release notes live in
[`omd-local/markdown-everything`](https://github.com/omd-local/markdown-everything).
