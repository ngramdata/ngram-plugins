---
name: create-video
description: Create a narrated AI video with ngram, such as an explainer, product demo, launch clip, or short. Use when the user asks to make, generate, or produce a video, or to turn text, a document, or a web page into one.
argument-hint: "[what the video should be about]"
---

# Create a video with ngram

Make a video for the user through the ngram tools. If `$ARGUMENTS` is given, it is the brief.

The tools describe their own inputs. This skill covers what the tools cannot tell you: how to treat the user's money, time, and output.

## Before anything is charged

Creating a video spends the user's ngram credits, priced per second of finished video. Nothing is spent until a create call succeeds, so settle everything first.

1. Prepare the video. Preparation is free and returns the settings ngram will use and the price.
2. Show the user the result in plain words: length, aspect ratio, style, voice, and the cost. Refer to styles and voices by name, never by id. If a length was requested, quote the total; if ngram is choosing the length, quote the per-second rate and say the total depends on the finished length.
3. Wait for a clear yes. A request to "make a video" is not consent to a price the user has not seen.
4. If the user changes anything after seeing the settings, prepare again and show the new result. Do not reuse an earlier confirmation for different settings.

Ask about a setting only when the choice matters to the user and they have not already stated it. Do not walk them through every option.

If the account cannot create videos, for example on a plan without access or with too few credits, say so plainly and point to the ngram app. Do not suggest ways around it.

## While it renders

A video takes minutes, sometimes many. After starting one:

- Give the user the job id and the project link right away, so they are not dependent on this conversation.
- Check progress at a relaxed pace. Progress moves in a few large steps and can sit on one value for most of the run; that is normal, not a stall.
- If the user would rather not wait, stop checking and tell them how to ask later.
- Never start a second video because the first seems slow or a call timed out. Check the status of the first one instead. A failed network call does not mean the video was not created.

Only cancel when the user asks. Credits already used by a cancelled video are not returned.

## When it is done

Give the user the video link and the project link. Then say two things briefly:

- Anyone who has the video link can open the file, so share it deliberately.
- Further edits, such as changing scenes or wording, happen in the ngram app through the project link. These tools create videos; they do not edit them.

If the video failed, report the reason the tool gave and ask before trying again.

## What not to promise

- A completion time.
- A script or storyboard to approve first. ngram plans and produces the video in one run.
- Editing, clipping, or translating an existing video.
