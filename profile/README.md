<p align="center">
  <img src="./assets/banner.png" alt="Artist Alley — self-hosted asset management for how studios produce, review, and archive work." width="820">
</p>

<p align="center">
  Self-hosted asset management for how studios produce, review, and archive work.<br>
  One binary, one database, one storage volume — everything from first concept to final delivery, in one place.
</p>

<p align="center">
  <a href="https://artist-alley.org">Website</a> ·
  <a href="https://artist-alley.org/docs/guides/install">Install</a> ·
  <a href="https://artist-alley.org/docs/guides/getting-started">Docs</a> ·
  <a href="https://github.com/Artist-Alley-Org/artist-alley">Source</a>
</p>

---

### What it is

A place to produce and archive, not just store files. Concept, modeling, rigging,
animation, cinematics, finals — in one self-hosted app, instead of spreading the work
across chat, shared drives, and file-transfer links.

The same model fits any team that catalogs things with media attached — museums,
libraries, galleries, archives. Tuned for production work, but general underneath.

### What's in the box

- **One viewer for everything** — images, video, audio, 3D, documents, and more, previewed in the browser and built for review.
- **Find anything fast** - full-text search across every asset, post, tag, and field.
- **Your metadata, your workflow** — custom fields with full history, and review states with an audit trail.
- **Built to federate** - pair two studios over signed, encrypted connections, and likes and comments cross between them. Sharing work across studios is planned.
- **Reads IIIF** — serves the IIIF standard, so deep-zoom and archive viewers work with your collections.
- **AI when you want it** - optional integrations, off by default, that connect to model servers or provider APIs you run or configure (embeddings, transcription, image editing). Experimental.

### Small core

One binary, one Postgres database, one storage volume: local disk or any S3-compatible
bucket. No message queue or microservices in the core. 3D preview thumbnails render inside
the main image, with no separate thumbnail container. Image-similarity search and
installable add-ons are planned, not available today.

### Repositories

| Repo | What it is |
|------|------------|
| [**artist-alley**](https://github.com/Artist-Alley-Org/artist-alley) | The application — Go + Postgres + SvelteKit. Start here. |
| [homebrew-tap](https://github.com/Artist-Alley-Org/homebrew-tap) | Reserved for Homebrew formulae; native packages are planned ([#286](https://github.com/Artist-Alley-Org/artist-alley/issues/286)). Install with Docker today. |
| [mviewer](https://github.com/Artist-Alley-Org/mviewer) | Rust-native viewer, converter, and glTF exporter for Marmoset `.mview` scenes. |

The remaining repositories are maintained forks of upstream Go libraries the app depends
on (glTF, SVG rasterizing, WebP, thumbhash, EPUB), pinned here for supply-chain safety.

### License

Open source and free to self-host, under **AGPL-3.0-only**. Commercial licensing and paid
tiers are planned but are not currently offered.
