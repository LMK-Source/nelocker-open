# nelocker-open — the exact prompts

> An asset you cannot regenerate is a lucky afternoon; a prompt you can re-run is a system.
> **Every image in `brand/` must be reproducible from this file.**
>
> Generated free by driving ChatGPT or Gemini through Claude-in-Chrome — not Replicate
> (`tools/genimage` is metered and is no longer the default). See LMK-STANDARD, Brand Kit.

Palette and refusals come from `BRAND.md`. **Change BRAND.md first, then the prompts.**

---

## icon-1024.png
_TODO_

```
TODO: state the hexes explicitly — a model drifts toward brighter, more saturated colour than the
brand allows unless the numbers are in the prompt.

Then the negative list from BRAND.md. It should be LONGER than the positive one: the category's
defaults are what an image model reaches for first.
```

## og-1200x630.png
_TODO_

Two rules learned building Sabrfy's:
1. State the ratio **and** the negative — "1200x630 landscape" alone comes back square. It took
   *"about 1.91:1 — landscape, definitely not square"*.
2. **Leave the text area bare.** Copy is composed over the image in code, never baked in, so the
   headline can change without regenerating art and stays crisp at every scale.

---

## Verification, before anything is committed
- **The 40px test**: downsample the icon to 40 and blow it back up. If it turns to mush it is a
  poster, not an icon.
- **Palette check**: sample the render and compare against BRAND.md's hexes.
- **Refusal check**: walk the "must never look like" list item by item.
