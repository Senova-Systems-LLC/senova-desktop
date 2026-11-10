# Open-source licenses

Senova is made by Senova Systems LLC. Its models and engines are built on the open-source projects
below, used under their licenses. Senova is not affiliated with or endorsed by these projects or their
authors. Connectors added from the gallery are downloaded by npm on request and keep their own licenses.

## Models

| Senova model | Built on | Author | License |
| --- | --- | --- | --- |
| Senova Prelude 1 | [gpt-oss-20b](https://huggingface.co/openai/gpt-oss-20b) | OpenAI | Apache-2.0 |
| Senova Étude 1 | [Flint 40B](https://ollama.com/library/flint) | Recursive | Apache-2.0 |
| Senova Suite 1 | [Qwen3.6 35B-A3B](https://huggingface.co/Qwen/Qwen3.6-35B-A3B) | Alibaba Qwen | Apache-2.0 |
| Senova Fugue 1 | [Laguna XS 2.1](https://huggingface.co/poolside/Laguna-XS-2.1) | Poolside | OpenMDW-1.1 |
| Senova Symphony 1 | [Qwen3.8 27B](https://huggingface.co/Qwen/Qwen3.8-27B) | Alibaba Qwen | Apache-2.0 |
| Senova Conductor 1 (picks a model in Auto, off by default) | [H2O-Lightning-4B](https://huggingface.co/h2oai/h2o-lightning-4b-gguf) | H2O.ai | Apache-2.0 |
| Senova Motif 1 (semantic search) | [Nomic Embed v1.5](https://huggingface.co/nomic-ai/nomic-embed-text-v1.5) | Nomic AI | Apache-2.0 |
| Senova Canvas 1 (images) | [FLUX.2 [klein] 4B](https://huggingface.co/black-forest-labs/FLUX.2-klein-4B), [FLUX.2 small decoder](https://huggingface.co/black-forest-labs/FLUX.2-small-decoder) | Black Forest Labs | Apache-2.0 |
| Senova Canvas 1 (prompt reader) | [Qwen3-4B](https://huggingface.co/Qwen/Qwen3-4B) | Alibaba Qwen | Apache-2.0 |
| Senova Aria 1 (voices) | [Kokoro-82M](https://huggingface.co/hexgrad/Kokoro-82M) | hexgrad | Apache-2.0 |
| Senova Notation 1 (dictation) | [Moonshine](https://github.com/moonshine-ai/moonshine) | Moonshine AI | MIT |

Where each model file is downloaded from is listed in `models/sources.json`.

## Engines

| Project | Used for | License |
| --- | --- | --- |
| [llama.cpp](https://github.com/ggml-org/llama.cpp) | Model engine | MIT |
| [Ollama](https://github.com/ollama/ollama) | Model engine | MIT |
| [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) | Speech engine | Apache-2.0 |
| [stable-diffusion.cpp](https://github.com/leejet/stable-diffusion.cpp) | Image engine | MIT |

## App

| Project | Used for | License |
| --- | --- | --- |
| [Next.js](https://github.com/vercel/next.js) | App framework | MIT |
| [React](https://github.com/facebook/react) | Interface | MIT |
| [prompt-kit](https://github.com/ibelick/prompt-kit) | Chat interface components | MIT |
| [Spec Kit](https://github.com/github/spec-kit) | The spec, plan, tasks, check flow behind Code's "Spec first" (ideas only, our own wording) | MIT |
| [shadcn/ui](https://github.com/shadcn-ui/ui) | Interface primitives | MIT |
| [Vercel AI SDK](https://github.com/vercel/ai) | Streaming chat | Apache-2.0 |
| [Model Context Protocol SDK](https://github.com/modelcontextprotocol/typescript-sdk) | Connectors | MIT |
| [xterm.js](https://github.com/xtermjs/xterm.js) | Terminal | MIT |
| [agent-desktop](https://github.com/vercel-labs/agent-desktop) (npm `agent-desktop` 1.1.0), by Vercel Labs | App control in the desktop app: reading a Windows app's accessibility tree and acting on its controls. Used unmodified as a separate program; it ships no NOTICE file. | Apache-2.0 ([license](https://www.apache.org/licenses/LICENSE-2.0)) |
| [esbuild](https://github.com/evanw/esbuild) | Artifact builds | MIT |
| [dagre](https://github.com/dagrejs/dagre) | Laying out Diagram studio artifacts | MIT |
| [unpdf (PDF.js)](https://github.com/unjs/unpdf) | Reading PDF files | MIT (PDF.js: Apache-2.0) |
| [mammoth](https://github.com/mwilliamson/mammoth.js) | Reading Word files | BSD-2-Clause |
| [JSZip](https://github.com/Stuk/jszip) | Reading Excel files | MIT |
| [Tesseract (tesseract.js)](https://github.com/naptha/tesseract.js) | Reading scanned pages | Apache-2.0 |
| [Tesseract English data](https://github.com/naptha/tessdata) | Reading scanned pages | Apache-2.0 (packaged under MIT) |
| [Freefield](https://github.com/neuregex/freefield) (commit 12012ec), Copyright (c) 2026 Sammir Femat (neuregex) | Create mode's design and app model: the Explore, app and workspace layouts, app names, summaries, template prompts and option phrases (`src/lib/create-apps.ts`, `src/lib/create-options.ts`, `src/components/senova/create/`), re-pointed at permissively licensed models | MIT (text below) |
| [Archivo](https://github.com/Omnibus-Type/Archivo), Copyright 2020 The Archivo Project Authors | Create mode's display type (`public/fonts/archivo.woff2`, licence in `public/fonts/archivo-OFL.txt`) | SIL OFL 1.1 |

## Artifacts

Senova's artifacts (documents, slides, sheets, charts, motion, diagrams, apps, designs, electronics, mechanical parts and agents) are its own code built
on these libraries. Nothing is copied from other AI products; only behaviour is reimplemented. The electronics schematic, PCB, simulator and Gerber writer, the design canvas and the agent flow engine are Senova's own code.

| Project | Used for | License |
| --- | --- | --- |
| [docx](https://github.com/dolanmiu/docx) | Word (.docx) export | MIT |
| [Tiptap](https://github.com/ueberdosis/tiptap) | Document editor | MIT |
| [docx-editor](https://github.com/eigenpal/docx-editor) by EigenPal: `@eigenpal/docx-editor-core`, `-react`, `-i18n`, `-agents` 1.9.0, used unmodified from npm | Paged Word editor for documents (pages, typing in the page, tracked changes). Only these Apache-2.0 packages are used; the repository's `packages/pro`, `editor-api`, `docx-to-pdf` and `telemetry` (EigenPal Pro Evaluation License) are not installed or copied. Its automatic Google Fonts lookup is switched off. | Apache-2.0 ([license](https://www.apache.org/licenses/LICENSE-2.0)) |
| [Univer](https://github.com/dream-num/univer) by DreamNum: `@univerjs/core`, `design`, `ui`, `themes`, `icons` (MIT), `engine-render`, `engine-formula`, `docs`, `docs-ui`, `drawing`, `rpc`, `protocol`, `telemetry`, `sheets`, `sheets-ui`, `sheets-formula`, `sheets-formula-ui`, `sheets-numfmt`, `sheets-numfmt-ui`, `sheets-filter`, `sheets-filter-ui`, `sheets-sort`, `sheets-sort-ui`, `sheets-conditional-formatting`, `sheets-conditional-formatting-ui`, `data-validation`, `sheets-data-validation`, `sheets-data-validation-ui`, `sheets-note`, `sheets-note-ui`, `thread-comment`, `thread-comment-ui`, `sheets-thread-comment`, `sheets-thread-comment-ui`, `find-replace`, `sheets-find-replace` 1.2.0, used unmodified from npm | Full spreadsheet editor for sheets. Only these open-source packages are used: none of Univer's closed Pro packages (`@univerjs-pro/*`: import/export, print, collaboration) or server services; nothing is registered for its telemetry interface. | Apache-2.0 ([license](https://www.apache.org/licenses/LICENSE-2.0)); `@univerjs/icons` MIT |
| [RxJS](https://github.com/ReactiveX/rxjs), [redi](https://github.com/wendellhu95/redi), [lodash-es](https://github.com/lodash/lodash), [decimal.js](https://github.com/MikeMcl/decimal.js), [rbush](https://github.com/mourner/rbush), [kdbush](https://github.com/mourner/kdbush), [ot-json1](https://github.com/ottypes/json1), [fast-diff](https://github.com/jhchen/fast-diff), [async-lock](https://github.com/rogierschouten/async-lock), [franc-min](https://github.com/wooorm/franc), [@flatten-js/interval-tree](https://github.com/alexbol99/flatten-interval-tree), [Floating UI](https://github.com/floating-ui/floating-ui), [cmdk](https://github.com/pacocoursey/cmdk), [class-variance-authority](https://github.com/joe-bell/cva), Radix UI (dialog, popover, dropdown-menu, hover-card, separator, slot, direction) | Parts the spreadsheet editor depends on | Apache-2.0 (RxJS, fast-diff, class-variance-authority), MIT, ISC (kdbush, ot-json1) |
| [ProseMirror](https://github.com/ProseMirror) (prosemirror-model, -state, -view, -transform, -commands, -history, -keymap, -tables, -dropcursor) | Editing engine under Tiptap and the paged editor | MIT |
| [docxtemplater](https://github.com/open-xml-templating/docxtemplater) (with [@xmldom/xmldom](https://github.com/xmldom/xmldom), MIT), [PizZip](https://github.com/open-xml-templating/pizzip) (with [pako](https://github.com/nodeca/pako), MIT and Zlib), [JSZip](https://github.com/Stuk/jszip), [xml-js](https://github.com/nashwaan/xml-js) (with [sax](https://github.com/isaacs/sax-js), BlueOak-1.0.0), [DOMPurify](https://github.com/cure53/DOMPurify), [sonner](https://github.com/emilkowalski/sonner), [clsx](https://github.com/lukeed/clsx), [Radix UI Select](https://github.com/radix-ui/primitives) | Parts the paged editor depends on | MIT (PizZip and JSZip are dual MIT or GPL-3.0 and used under MIT; DOMPurify is dual MPL-2.0 or Apache-2.0 and used under Apache-2.0) |
| [marked](https://github.com/markedjs/marked) | Markdown parsing for exports | MIT |
| [KaTeX](https://github.com/KaTeX/KaTeX) (with its mhchem and copy-tex extensions) | Math and chemistry in chat and documents | MIT |
| [MathJax](https://github.com/mathjax/MathJax-src) 3.2.2 (`mathjax-full`, with [mhchemParser](https://github.com/mhchem/mhchemParser), Apache-2.0) | Equations drawn as outlines in Explainer artifacts | Apache-2.0 ([license](https://www.apache.org/licenses/LICENSE-2.0)) |
| [Manim](https://github.com/3b1b/manim), Copyright (c) 2018-2026 3Blue1Brown LLC, and [Manim Community](https://github.com/ManimCommunity/manim), Copyright (c) 2024 the Manim Community Developers | The animation vocabulary of Explainer artifacts (create, write, transform, matching equation symbols, indicate, value trackers). No Manim code, scenes, videos or branding are used; the explainer engine (`src/lib/explainer`) is Senova's own code. | MIT |
| [CodeMirror](https://github.com/codemirror/dev) (via [@uiw/react-codemirror](https://github.com/uiwjs/react-codemirror)) | Source editing | MIT |
| [PptxGenJS](https://github.com/gitbrent/PptxGenJS) | PowerPoint (.pptx) export | MIT |
| [Mermaid](https://github.com/mermaid-js/mermaid) | Diagrams | MIT |
| [anime.js](https://github.com/juliangarnier/anime) | Motion artifacts | MIT |
| [transitions-dev](https://github.com/Jakubantalik/transitions-dev) (commit 038b0bd), Copyright (c) 2026 Jakub Antalík | Easing curves and timings behind the Motion presets (`artifact-runtime/motion-presets.js`) | MIT |
| [motionmaxxing](https://github.com/Tejashmakwana/motionmaxxing), made by Tejas Makwana | Motion direction for Motion artifacts (timing, easing, type, layout, transitions, pacing, the close) and the Senova.fx moves, adapted and paraphrased, modified by Senova Systems LLC. Its NOTICE: "motionmaxxing: looksmaxxing for motion graphics. Made by Tejas Makwana (x.com/makwanatejas170) · github.com/Tejashmakwana/motionmaxxing". GSAP, which that repository bundles, is not used. | Apache-2.0 ([license](https://www.apache.org/licenses/LICENSE-2.0)) |
| [mp4-muxer](https://github.com/Vanilagy/mp4-muxer) / [webm-muxer](https://github.com/Vanilagy/webm-muxer) | Video export | MIT |
| [Tailwind CSS](https://github.com/tailwindlabs/tailwindcss) | Styling inside artifacts | MIT |
| [Recharts](https://github.com/recharts/recharts) | Charts inside React artifacts | MIT |
| [Lucide](https://github.com/lucide-icons/lucide) | Icons inside artifacts | ISC |
| [docx-preview](https://github.com/VolodymyrBaydalka/docxjs) | Showing Word files | Apache-2.0 |
| [Apache ECharts](https://github.com/apache/echarts) (with [ZRender](https://github.com/ecomfe/zrender), BSD-3-Clause) | Chart artifacts | Apache-2.0 |
| [formula.js](https://github.com/formulajs/formulajs) (with [jStat](https://github.com/jstat/jstat), MIT, and [bessel](https://github.com/SheetJS/bessel), Apache-2.0) | Spreadsheet functions | MIT |
| [SheetJS Community Edition](https://git.sheetjs.com/sheetjs/sheetjs) | Reading Excel files and Excel (.xlsx) export | Apache-2.0 |
| [gifenc](https://github.com/mattdesl/gifenc) | GIF export for Motion | MIT |
| [three.js](https://github.com/mrdoob/three.js) | 3D view in Mechanical artifacts | MIT |
| [three-bvh-csg](https://github.com/gkjohnson/three-bvh-csg) and [three-mesh-bvh](https://github.com/gkjohnson/three-mesh-bvh) | Solid modelling (union, cut, intersect) in Mechanical artifacts | MIT |
| [pdf-lib](https://github.com/Hopding/pdf-lib) (with [pako](https://github.com/nodeca/pako), MIT and Zlib) | PDF tools: merge, split, fill, sign, redact | MIT |
| Deck fonts from [Google Fonts](https://fonts.google.com): Inter, DM Sans, Manrope, Outfit, Work Sans, Space Grotesk, IBM Plex Sans, Montserrat, Poppins, Nunito, Raleway, Open Sans, Syne, Fraunces, Playfair Display, DM Serif Display, Lora, Merriweather, Source Serif 4, Libre Baskerville, IBM Plex Serif, Crimson Pro, Instrument Serif, Bebas Neue, Archivo Black, JetBrains Mono, Space Mono; Roboto | Fonts a deck's style line may name. Not shipped with Senova: fetched once by Senova's server when a deck uses them, kept in `~/.senova/artifacts/deck-fonts` and embedded unmodified in that deck's page, so the slide frame never contacts Google (`src/lib/server/deck-fonts.ts`) | SIL Open Font License 1.1; Roboto Apache-2.0 / OFL-1.1 |

## Weak-copyleft parts

Senova uses no strong-copyleft code. These parts have file-level (weak) copyleft licences. Each is used
unmodified as published, and its source is at the link given.

| Project | Where | License | Ships in the desktop installer? |
| --- | --- | --- | --- |
| [elkjs](https://github.com/kieler/elkjs) 0.9.3, a dependency of Mermaid | Diagram layout code inside the Mermaid bundle for artifacts (`mermaid-inline.js`) | EPL-2.0 | Yes, unmodified. Source: https://github.com/kieler/elkjs/tree/0.9.3 |
| [sharp](https://github.com/lovell/sharp) prebuilt libvips (`@img/sharp-*`), an optional dependency of Next.js | Next.js image optimisation, which Senova does not use (`images.unoptimized` in `next.config.ts`) | Apache-2.0 and LGPL-3.0-or-later | No. The installer leaves it out (`desktop/electron-builder.yml`) |
| [lightningcss](https://github.com/parcel-bundler/lightningcss) | Tailwind's CSS compiler, used only at build time | MPL-2.0 | No (build tool) |
| [axe-core](https://github.com/dequelabs/axe-core) | Accessibility lint rules, development only | MPL-2.0 | No (development tool) |
| FFmpeg (`ffmpeg.dll`, built by the Electron project without patent-encumbered codecs) | Audio and video playback in the Windows app's window, part of Electron | LGPL-2.1-or-later | Yes, unmodified, as a separate DLL. Source: https://github.com/electron/electron and https://ffmpeg.org |

## Windows app

| Project | Used for | License |
| --- | --- | --- |
| [Electron](https://github.com/electron/electron) 45 (with Chromium; its full licence list ships as `LICENSES.chromium.html` in the install folder) | The Windows app's window and tray | MIT (Chromium: BSD-3-Clause and others) |
| [Node.js](https://github.com/nodejs/node) 24 (`resources/node/node.exe`, licence beside it) | Runs Senova's local app server | MIT and others listed in its LICENSE |
| [electron-builder](https://github.com/electron-userland/electron-builder) and [electron-updater](https://github.com/electron-userland/electron-builder/tree/master/packages/electron-updater) | Installer and signed updates | MIT |
| [electron-log](https://github.com/megahertz/electron-log) | Logs kept on this PC | MIT |

## Freefield licence

```
MIT License

Copyright (c) 2026 Sammir Femat (neuregex)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
