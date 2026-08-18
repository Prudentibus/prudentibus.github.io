# prudentibus.github.io

Neon channel-wall portfolio — each project is a "channel" of stacked full-width screenshots, switched with a portal wipe. Live at https://prudentibus.github.io

| Path | Description |
|------|-------------|
| [INDEX.md](INDEX.md) | This index. |
| [index.html](index.html) | The whole site, self-contained (inline CSS/JS): neon navbar (JP→EN typewriter brand, left-to-right tube-flicker intro, portal slider under active tab, scroll-progress tube), channel switching (scanline reveal on first load, direction-aware portal wipe after; keyboard ← → and number keys), contact channel pinned last (pink identity, paper-plane tab icon), OPEN LIVE button that goes unlit on channels without a link, compact-nav breakpoints ≤1000px/≤760px and a rotate-your-phone prompt on portrait phones. Google Fonts (DotGothic16, Noto Sans JP). |
| [projects.js](projects.js) | Manual config, one entry per project: `name` (nav tab), `link` (live site; "" unlights OPEN LIVE), `folder`, optional filename `prefix`. Screenshots are auto-discovered by numeric index ({prefix}1 / {prefix}01, .png/.jpg/.jpeg/.webp/.svg) and stack top-to-bottom; discovery stops at the first missing number, so keep numbering gapless. |
| [assets/](assets/) | One folder per project holding its numbered screenshot chunks (JPEG q88, 1920px wide) consumed by the discovery above. |
