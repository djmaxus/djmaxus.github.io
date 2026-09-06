---
layout: post
title: "It's almost TOO easy to make a good poster with Typst"
categories: dev
---

**TL;DR** I recently did so for the first time:
[github:djmaxus/ecmor-2026/poster](https://github.com/djmaxus/ecmor-2026/tree/main/poster/).
Turns out, with **Typst**, a modern typesetting tool, you won't even need any special package like `piece-of-posters`.
After years of $\LaTeX$ and, forgive me, Microsoft Office, I don't want to go back.
You might going to want to switch from $\LaTeX$, too, or skip it entirely.
At least for serious work.

## Preamble

While any LLM can tell you a lot about all the pros and cons of Typst compared to LaTeX and PowerPoint, I'd like to serve as a real-wold example.

- almost any content can go anywhere; this makes setting custom backgrounds provided by your conference very straightforward
- piece-of-posters is useless;
  - default themes add unnecessary visuals and sometimes even noise
  - still require a lot of customisation you'd do anyway
    - font sizing
    - multi-column text
    - theme updates to reduce the said visual noise
    - lack of abstractions for author-organisation correspondence, unlike LaTeX
      - no abstractions for contact info and links
  - The same can be achieved by adjsuting the fonts for body text, title, and lower-level headers
    - you'd preserve the adaptive content distribution between columns
    - conventional bibliographic references are too much for a poster; that can be a whole another take on whether we as a community could come up with a reference style more well-suited for how we actually publish and access research.
      - Authors, year, title, url of the source
- math typesetting was harder to start to get used to than I anticipated
  - this is where Typst stepped rather too far away from LaTeX, and the LaTeX math rendering is not supported (at least within Typost itself)
  - although now it seems I just should've read the manual instead of jumping right into it
- Typst is small, unlike gigabytes of LaTeX with the full suite of packages
  - fast
  - one entry point for everything you need to do
    - show my phd thesis pdf build command
  - packages are available at the registry or you can get them from whatever and connect to your project
  - I already printed my poster when noticed commas between some of the images: I though they were required to
  - accepts vector and raster images: png, svg, pdf
  - compiles easily and customizably to pdf, svg, and png; that's how I can embed my poster directly to README.md
- approach of functions and variables that can be declared at any point
- declaration of defaults for commands that apply downstream until redefined again
- good tooling: LSP with syntax hints and autocomplete, preview that is
  - fast
  - interactive both ways
  - does not pollute your working folder

## Journals still require $\LaTeX$

Funny enough, the use of $\LaTeX$ seems to be considered a bold, hi-tech move for many.

Well, that's a tricky one. There are many other shifts happening in the world of scientific publications, the biggest being the rise of LLMs. That alone seems to be about to change a lot how we produce communicate science. What are the chances a LaTeX successor might as well make its way in? Maybe not Typst in particular, but it is definitely a step in the right direction.

[![brainmade](/black-logo.svg)](https://brainmade.org/)
