# ngram plugin for Cursor

Create narrated AI videos and business images with [ngram](https://www.ngram.com) from Cursor.

The plugin connects Cursor to your ngram account and adds two skills that keep you in control of what is spent:

- **create-video**: previews the settings and cost, waits for your yes, then starts the video and gives you the link when it is done.
- **create-image**: confirms what will be made before generating or editing a product, brand, or marketing image.

You need an ngram account with credits; the cost is shown before anything is created. Free accounts work too: their videos carry the ngram watermark and end card.

## What it contains

- One hosted MCP server, `https://mcp.ngram.com`, over HTTPS.
- Two skills, `create-video` and `create-image`.

It has no hooks, no scripts, and no local commands, and it installs nothing on your machine.

## Network and credentials

- The plugin calls `https://mcp.ngram.com` and nothing else.
- Sign-in is OAuth with your ngram account on first connect. The plugin stores no API key and reads no environment variables, files, or tokens from your machine.
- Finished videos are served from `https://www.ngram.com`. Finished images are served from ngram's asset storage.

ngram's privacy policy is at https://www.ngram.com/privacy.

## Use

Ask in plain words:

- "Make me a 15-second video explaining what a prime number is."
- "Turn this article into a one-minute explainer: https://example.com/post"
- "Create a square social post announcing the launch of our note-taking app, Quill."
- "Is my video ready?"

## Good to know

- Videos take several minutes. You get a job id and a project link as soon as one starts, so you do not have to wait in the conversation.
- Anyone who has a finished video or image link can open the file.
- Images are for business use: product, brand, and marketing visuals. ngram declines images with no such purpose.
- These tools create videos and images. Editing a finished video happens in the ngram app, through the project link.

## Support

Documentation: https://www.ngram.com/docs/mcp · Contact: https://www.ngram.com/contact

## License

MIT
