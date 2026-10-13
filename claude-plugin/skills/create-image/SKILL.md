---
name: create-image
description: Create or edit a business image with ngram, such as a product visual, ad, launch graphic, social post, or thumbnail for a brand, product, or campaign. Use when the user asks to generate, design, or edit a marketing or product image and wants it made through ngram.
argument-hint: "[what the image should show and what it is for]"
---

# Create an image with ngram

Make or edit an image for the user through the ngram tools. If `$ARGUMENTS` is given, it is the brief.

The tools describe their own inputs. This skill covers what they cannot tell you: what ngram will accept, and how to handle the user's credits and output.

## What ngram makes

ngram creates images for business and commercial work: product and brand visuals, ads, launch and campaign graphics, website and social assets, pitch visuals, and thumbnails. It declines images with no business, product, brand, or marketing purpose, and the refusal reads as a generic content-policy message.

So before generating:

- Say in the prompt what the image is for and whose product, brand, or campaign it serves, using what the user told you. Do not invent a brand or a purpose the user did not give.
- If the request is plainly personal or decorative, such as a pet portrait or a fantasy landscape, tell the user ngram is built for business visuals and ask whether there is a product or campaign behind it. Do not send it anyway.

## Before generating

Creating or editing an image can spend the user's ngram credits, depending on their plan.

1. Restate what you are about to make in one or two lines: the subject, the shape, what it is for, and any style or template you chose. Name styles and templates by name, never by id.
2. Wait for the user to agree before the first generation in a conversation. Once they have agreed to a direction, small variations on it do not need a fresh yes each time.
3. For an edit, confirm which image is being changed and what should stay the same.

ngram applies the account's default brand kit, including its logo, unless brand styling is turned off. When the image is for a brand or product other than the one that kit belongs to, turn brand styling off, or the result will carry the wrong logo and colours. If you cannot tell whose kit it is, ask.

Look up models, shapes, styles, or templates only when the user's request depends on one of them. Otherwise let ngram choose.

## After generating

- Images finish quickly but not instantly. If the result is not ready, check its status rather than generating again.
- Give the user the image link. Anyone who has the link can open the file, so share it deliberately.
- If ngram refuses the request, report its message, then explain the likely cause in plain words: the request probably did not read as a business or marketing image. Ask what the image is for before trying again. Do not retry the same prompt, and do not reword it to slip past the check.
- If it failed for another reason, report what the tool said and ask before retrying.

Do not generate images of real people the user has no right to depict, and do not upload or reference source images the user has not provided or pointed to.
