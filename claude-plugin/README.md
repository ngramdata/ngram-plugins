# ngram plugin for Claude

Create narrated AI videos and business images with [ngram](https://www.ngram.com) from Claude Code and Claude (claude.ai).

The plugin connects Claude to your ngram account and adds two skills that keep you in control of what is spent:

- **create-video**: previews the settings and cost, waits for your yes, then starts the video and gives you the link when it is done.
- **create-image**: confirms what will be made before generating or editing a product, brand, or marketing image.

You need an ngram account with credits; the cost is shown before anything is created. Free accounts work too: their videos carry the ngram watermark and end card.

## Install

### Claude Code

```
/plugin marketplace add ngramdata/ngram-plugins
/plugin install ngram@ngram
```

Then run `/mcp`, choose the ngram server, and sign in with your ngram account.

### Claude (claude.ai)

Open **Customize → Plugins → Add → Add marketplace**, choose **Add from a repository** and enter `ngramdata/ngram-plugins`, then add **ngram** from it. Open the plugin's **Connectors** tab, connect **ngram**, and sign in with your ngram account.

A plugin added on claude.ai also appears in Claude Code when you are signed in to the same account.

## Use

Ask in plain words:

- "Make me a 15-second video explaining what a prime number is."
- "Turn this article into a one-minute explainer: https://example.com/post"
- "Create a square social post announcing the launch of our note-taking app, Quill."
- "Is my video ready?"

In Claude Code you can also call the skills directly with `/ngram:create-video` and `/ngram:create-image`.

## Good to know

- Finished videos and images show inline in the conversation on Claude (claude.ai), with the links beside them.
- Videos take several minutes. Claude gives you a job id and a project link as soon as one starts, so you do not have to wait in the conversation.
- Anyone who has a finished video or image link can open the file.
- Images are for business use: product, brand, and marketing visuals. ngram declines images with no such purpose.
- The plugin sends your requests to ngram at `https://mcp.ngram.com/claude` and nowhere else. ngram's privacy policy is at https://www.ngram.com/privacy.
- These tools create videos and images. Editing a finished video happens in the ngram app, through the project link.

## Support

Documentation: https://www.ngram.com/docs/mcp · Contact: https://www.ngram.com/contact

## License

MIT
