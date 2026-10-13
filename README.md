# ngram plugins

Official [ngram](https://www.ngram.com) plugins for AI coding assistants. A plugin connects the assistant to your ngram account so you can create narrated AI videos and business images by asking, and adds two skills that show the settings and cost and wait for your yes before anything is created.

| Assistant | Folder                             |
| --------- | ---------------------------------- |
| Cursor    | [`cursor-plugin`](./cursor-plugin) |
| Claude    | [`claude-plugin`](./claude-plugin) |

## What a plugin contains

- One hosted MCP server on `https://mcp.ngram.com`, over HTTPS.
- Two skills, `create-video` and `create-image`.

There are no hooks, no scripts and no local commands, and nothing is installed on your machine.

## Network and credentials

- A plugin calls `https://mcp.ngram.com` and nothing else.
- Sign-in is OAuth with your ngram account on first connect. No API key is stored, and no environment variables, files or tokens are read from your machine.

ngram's privacy policy is at https://www.ngram.com/privacy.

## About this repository

It is generated from ngram's main codebase and overwritten on each release, so pull requests here cannot be merged. Send questions and problems to https://www.ngram.com/contact.

## License

MIT
