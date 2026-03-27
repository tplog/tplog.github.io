---
title: "Maybe HTML Is a Better Source Format for the AI Era"
description: "Why HTML may be a better source format than Markdown when the real goal is to deliver polished content people can actually read and use."
pubDate: "Mar 27 2026"
tags: ["ai", "html", "markdown"]
---

Lately, while building AI workflows, I’ve started to rethink an assumption that used to feel almost obviously true:

**Is Markdown really the best content format for us?**

Over the past few years, people have more or less settled on a consensus: Markdown is simple enough, light enough, and universal enough that it naturally works as a container for knowledge, documentation, blog posts, manuals, and even AI-generated intermediate artifacts.

But recently I’ve started to feel the opposite.

**If the goal is to show something to other people, HTML may actually be a better final source format than Markdown.**

Not because HTML is more advanced, but because I’m starting to realize something else:

**When we build something, the intermediate artifact often matters less than we think. In the end, what people actually want to see is the result.**

## Where this idea came from

This started when our company publicly released a skill.

Its job is very specific: it guides us in creating posters, intro pages, and other materials meant to be seen by other people. And the output it generates is highly aligned with the company’s brand standards.

After using it in practice, my reaction was pretty direct:

**If a piece of content is meant to be shown to someone else, the result after going through this kind of skill is obviously more human-friendly than ordinary Markdown.**

“Human-friendly” here does not mean easier to write. It means:

- it is much closer to the final presentation,
- it aligns better with brand standards,
- its layout, hierarchy, and visual rhythm feel more complete,
- and readers do not have to mentally reconstruct what it is *supposed* to look like after rendering.

In other words, maybe what AI really amplifies is not the ability to write Markdown faster, but the ability to **produce the result directly**.

## I’m starting to wonder if we care too much about the intermediate format

In the past, we spent a lot of attention on the middle layer:

- which editor to use,
- how collaboration should work,
- how permissions should be managed,
- how formats stay compatible,
- how to make Markdown more standardized.

All of those things matter. But I increasingly suspect that:

**They matter because they serve the outcome, not because they are the outcome.**

Take Notion, for example.

People often describe its value in terms of collaboration, editing, permissions, databases, and block-based composition.

But if you take a step back, the thing that actually matters most is not any one of those features.

It is this:

**Notion ultimately exists as a knowledge base.**

Put differently, what users really need is not “something that is easy to edit.” What they need is **a knowledge object that can ultimately be read, stored, delivered, and accessed over time.**

From that perspective, many of the supporting systems we used to treat as inseparable from the content itself may not actually need to live inside the content body at all.

## If the core of content is the result, HTML changes position

Once you put the *result* at the center, the role of HTML changes.

Traditionally, we think of HTML as an output format:

- Markdown is the source,
- HTML is the rendered result,
- PDF is the export.

But lately I’ve started to think that, at least for one category of content, a more reasonable relationship might be this:

- **HTML is the source itself**
- **PDF is an exported version of HTML**
- **Collaboration, discussion, and approval happen outside the content body**

That shift has several very direct advantages.

## 1. The source file and the result are no longer separate

If the final user sees HTML, then using HTML as the source means:

**What you see is the content itself.**

You no longer need to go through the extra translation step of “write Markdown first, then imagine how it will eventually be rendered.”

That removes a very common misalignment:

The author writes an abstract structure, while the reader sees a concrete result. But during writing, the author was never really confronting that final result directly.

An HTML-first approach forces the author to face the final presentation from the very beginning.

## 2. Brand expression becomes much stronger by default

Markdown’s strength is simplicity. But its weakness is just as obvious:

**It is great for carrying structured text, but it is not naturally suited for content with strong presentation requirements.**

As soon as your content needs things like:

- stronger visual hierarchy,
- clearer brand rules,
- more expressive components,
- more complex layout structures,
- higher-quality external presentation,

Markdown quickly turns into a format that is only *barely good enough*.

And then you usually start doing things like:

- adding custom Markdown syntax,
- embedding raw HTML,
- switching to MDX,
- introducing extra rendering conventions,
- writing a lot of post-processing logic.

At that point, the reality is simple:

**On the surface you are still using Markdown, but in practice you are already taking a long detour to write HTML indirectly.**

If that is true, it may be better to just admit that HTML is the layer actually carrying the burden of expression.

## 3. HTML feels more like a deliverable asset than a rendering byproduct

This is probably the strongest feeling I’ve had recently.

A lot of the time, we design content systems as if they were mainly **editor systems**, instead of thinking of them as **asset systems**.

But if a piece of content is ultimately meant to:

- be sent to other people,
- live in a knowledge base,
- serve as external-facing material,
- be exported as a PDF,
- be stored for the long term,
- be reused later by another AI or another human,

then it behaves much more like a **deliverable asset** than a temporary state inside a writing process.

And HTML has a natural advantage here:

**It can be consumed directly by the browser, exported naturally into PDF, and still preserve much richer semantic and presentation information than Markdown.**

In other words, it does not feel like an intermediate format. It feels much closer to the primary form of the content itself.

## 4. Collaboration does not necessarily need to be embedded in the content file

A common objection comes up immediately:

“What about collaboration? Comments? Permissions?”

Those are real concerns.

But I now think collaboration does not have to be tightly bound to the content body itself.

We became accustomed to tools like Notion because they compress all of the following into one system:

- content,
- collaboration,
- permissions,
- comments,
- workflow.

That is convenient. But it also makes it easy to assume that:

**Content must exist inside a collaboration system.**

I’m no longer sure that is true.

You can absolutely split them apart:

- the content body is HTML,
- one HTML version is preserved for external use,
- one PDF version is exported for delivery,
- and collaboration, discussion, review, and annotations happen in separate systems.

That can actually make the content more stable.

Because collaboration systems change. Workflow tools change. Permission models change.

But a final HTML document and a final PDF deliverable are often much closer to the thing that is truly worth preserving over time.

## AI may make this trend much more obvious

Without AI, an HTML-first approach might sound like a choice that is more refined, but also more troublesome.

With AI, the situation changes.

Because AI is especially good at producing a result directly.

This is even more true in situations where:

- brand rules are clear,
- components and layout patterns are stable,
- presentation templates are consistent,
- the output is meant to be seen by others.

In those cases, AI is not really helping you “write Markdown faster.”

It is helping you **generate a result that is already close to deliverable quality, much faster**.

Once that becomes possible, the value of Markdown as an intermediate layer starts to decline.

You no longer need to first write an abstract, plain, waiting-to-be-rendered version.

What you really want is this:

**To get the final piece directly—something already good enough, polished enough, and aligned enough with brand expectations.**

## So my current simple view is this

For a certain class of content that is explicitly **meant to be seen by other people**, especially things like:

- posters,
- landing or intro pages,
- branded content,
- external explanation materials,
- knowledge documents with visual requirements,

maybe the more reasonable workflow is:

1. **Treat HTML as the actual content source**
2. **Export a PDF version from the HTML**
3. **Keep collaboration and workflow outside the content itself**

This is obviously not right for every scenario.

If you are just taking quick notes, writing a README, or drafting internal technical thoughts, Markdown is still excellent.

But if your goal was never “write an intermediate text file” in the first place, and was always “deliver a final result,” then HTML’s role may need to be reconsidered.

It is not just the rendering endpoint.

It may actually be the content body.

## Closing thought

I have not fully thought this through yet, but at least one judgment is becoming clearer for me:

**We have spent too long designing content systems around the editing experience. In the future, we may need to design them more around the final result.**

If that is true, then Markdown represents an **input-first** way of thinking,
while HTML may represent a **result-first** way of thinking.

And in the AI era, the latter may matter more and more.
