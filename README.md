# amplification-ecco

Source for **amplification.etherealconnectionsco.com** — the ECCO
Amplification Surface. A multi-subject editorial surface where each
independent builder ECCO amplifies is presented as a paired structure:
a Tier II trailer (ECCO-authored editorial layer) at a stable
subdirectory beneath the parent, and a Tier III substance page
(originator-owned) at the originator's own domain. *Provenance
preserved. Right of refusal explicit. Doctrine over excuse.*

**First subject:** Derek Antoine Lee · Bonded Science · Tier II trailer
at `/echo.bonded/` on this surface, Tier III substance at
`bonded.etherealconnectionsco.com` (originator-owned · ECCO-built
under a service arrangement with Derek).

## Posture

**Public repository.** The Amplification Surface hosts ECCO's
editorial amplifications of independent builders, with each subject's
ECCO-authored trailer maintained as a self-contained `/echo.X/`
subdirectory. Visibility supports verification of each amplification's
record, demonstration of ECCO's amplification posture, and preservation
of an independent timestamped reference for ECCO's editorial layer.
Licensed under
[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) —
read, cite, link, share for non-commercial purposes; do not repackage
or rebrand. See `LICENSE` for full terms.

**Third-party amplification carve-out.** Each subject amplified on
this surface is presented in two parts: a Tier II trailer
(ECCO-authored editorial layer) at a `/echo.X/` subdirectory beneath
the parent, and a Tier III substance page (originator-owned) at the
originator's own domain. The first subject is the Bonded Science
framework of Derek Antoine Lee (@treeminded / @derekantoinelee) —
Tier II trailer at `/echo.bonded/` on this surface, Tier III substance
at `bonded.etherealconnectionsco.com`. **The underlying work of any
amplified subject is NOT included in the CC BY-NC-ND 4.0 grant.** Each
subject's materials remain that subject's property — referenced here
for editorial commentary and amplification, with the originator's
permission where a collaboration is named (as with Bonded) — and
may not be reproduced, excerpted, or redistributed without separate
written permission from the originator.

For the Bonded subject specifically: the architecture animation
embedded inside `/echo.bonded/index.html` (as H.264-encoded base64
video) is a representation of Derek's Bonded Science framework.
Consistent with the Builder Statement in Derek's own Tier III
`LICENSE`, **ECCO holds no rights to the animation** — or to the
architecture, the diagrams, or any other representation of the
science. The animation is **not** part of the CC BY-NC-ND 4.0 grant;
all rights in it are reserved to Derek Antoine Lee. The line is clear:
ECCO's editorial framing, design system, and doctrinal commentary are
ECCO's and CC-licensed; the subject's underlying work — and every
representation of it — belongs to the originator. The same rule
applies to any subsequent subject.

**Posture: collaboration, named.** As a surface default, an ECCO
amplification is an unsolicited act of editorial amplification unless
the subject's collaboration is explicitly named. For the Bonded
subject, the collaboration is named: ECCO designed, builds, and hosts
Derek's Tier III surface (`bonded.etherealconnectionsco.com`) under a
service arrangement with him, and the Bonded amplification is
published with Derek Antoine Lee's consent. It is not unsolicited.
Each subject's right of refusal is preserved regardless — if a
subject requests their amplification be modified or taken down, it
will be. Provenance stays with the originator, including the
originator's authority over whether and how amplification is welcome.

The build pipeline runs against the same `check-links.mjs` v4 gate as
the rest of ECCO so the doctrine is enforced uniformly — the integrity
is structural across every surface, public or private.

## Doctrine

> Every external claim verifiable. Every link live.
> Live = reachable by a human in a browser. Not "reachable by every bot."

The build pipeline enforces this. A push that introduces a dead external
URL fails the build before it can ship; the last good version stays live.

## What the gate catches on this surface

The Amplification Surface currently ships the parent surface
(`/index.html`), a custom 404 page, and the Bonded Tier II trailer
(`/echo.bonded/index.html`). The originator's Tier III substance lives
at `bonded.etherealconnectionsco.com` — an independent surface under
Derek's own editorial authority with its own build gate; outside this
repo's check-list. Additional subjects will add their own `/echo.X/`
trailer subdirectories here, and (typically) their own external
domains for substance.

The external citations on this surface — and how each is held to the
doctrine (the gate fetches `http(s)://` URLs only; bare text references
and ECCO's own subdomains are carried by quarterly editorial review):

**Bonded Tier II trailer** (`/echo.bonded/index.html`):

- Five Zenodo DOIs (Bonded Science publication record) — linked on the
  trailer as `https://doi.org/…` URLs and verified by the link gate.
  (Derek's own Tier III surface links the same five the same way.)
  - `https://doi.org/10.5281/zenodo.18648464` (Entropy Is Not Destiny, 2026)
  - `https://doi.org/10.5281/zenodo.17526990` (Grid Guard Pulse Cooling System, 2025)
  - `https://doi.org/10.5281/zenodo.17117311` (GridGuard Pulse Emergency Resilience, 2025)
  - `https://doi.org/10.5281/zenodo.18425113` (Field Preservation Pre-Entropy Stabilization, 2026)
  - `https://doi.org/10.5281/zenodo.17969880` (Magnetic Cooling Blueprint, 2025)
- USPTO patent reference: `US19438644` (text reference inside the
  trailer; not currently linked — text claim subject to quarterly
  editorial review, not the link gate)
- Derek's Tier III substance domain: `bonded.etherealconnectionsco.com`
- Derek's Instagram handles: `@treeminded`, `@derekantoinelee`

**Surface-wide** (parent + 404):

- ECCO main site: `etherealconnectionsco.com`
- ECCO Instagram handle: `@etherealconnectionsco`
- Mailto: `jeremiah@etherealconnectionsco.com`
- Google Chrome download URL (referenced by the Chrome detection banner)
- ECCO LinkedIn company page: `linkedin.com/company/113015173`
- Founder LinkedIn: `linkedin.com/in/jeremiah-hearne-b0611413`
- Founder's artist Instagram handle: `@ardezen.co`

Some institutional or platform URLs may return 403/999 to cloud-runner
traffic (anti-bot policy) — those are logged as TOLERATED and the
build passes. The doctrine here is the same as on every other ECCO
public surface: mechanical enforcement where possible, named limitations
where it isn't, quarterly editorial review across every external citation
regardless.

## Build

```
node check-links.mjs index.html echo.bonded/index.html 404.html
```

Runs on Netlify Node 20, no local install required. Auto-deploys on push
to `main`. Configuration in `netlify.toml`.

> **Note on the build command:** The build gate runs against the parent
> `index.html` (Amplification umbrella), the Bonded Tier II trailer, and
> the 404. Each additional subject adds one more `/echo.X/index.html`
> argument to the command in `netlify.toml` when its trailer lands.
> Tier III substance pages live at originator-owned domains and run
> their own build gates; they are not arguments to this repo's
> check-list.

Status taxonomy:
- **OK** (2xx / 3xx) — verified live.
- **TOLERATED** (401 / 403 / 451 / 999, or any non-2xx from the cloud-block
  whitelist) — site refuses automation but resolves for humans. Logged,
  build passes.
- **BROKEN** (other 4xx / 5xx / network error) — build fails.

## Files

| File | Purpose |
|------|---------|
| `index.html` | **Amplification umbrella landing** — Tier I parent surface. Hybrid ceremonial-gate-into-archive-register. Pulsing flower-of-life bloom (Seed-of-Life inside seal, Flower-of-Life around seal, concentric cosmos rings beyond) gates into the archive register with manifesto, three-tier explainer (Soil · Seed · Fruit construction sequence), current entries (Bonded as Entry 01), and inclusion CTA. Surface posture, doctrine line, footer. |
| `404.html` | Custom 404 — Amplification design register (propagating-signal sigil unique to this entry gate), surface-agnostic copy, returns to the parent archive. Covers all subjects. |
| `echo.bonded/index.html` | **Bonded Tier II trailer** — ECCO-authored editorial trailer for the Bonded subject. Immersive Field-Note register; the architecture animation is embedded as H.264 base64 video directly in the file (single-file portable). End-of-trailer CTAs forward to Derek's Tier III substance at `bonded.etherealconnectionsco.com` and ECCO Instagram. The Bonded amplification's named-collaboration posture is stated on the parent surface. |
| `echo.bonded/` (aux) | Per-subject portability kit — `404.html`, `LICENSE`, `README.md`, `netlify.toml`, `check-links.mjs`, `.gitignore`. Inactive while nested under the parent (the parent's config governs); carry-along artifacts for future subdomain extraction (Master Context pattern). |
| `check-links.mjs` | Build-gate link integrity checker (v4) |
| `netlify.toml` | Build configuration |
| `LICENSE` | CC BY-NC-ND 4.0 (with per-subject amplification carve-outs preserving each originator's underlying work) |
| `.gitignore` | Standard exclusions |

> **Note on local filenames:** Trailer pages in active local
> development may carry working names like `field_note_03.html` or
> `bonded_landing_v2.html`. Each must be renamed to `index.html`
> inside its own `/echo.X/` subdirectory before commit — Netlify
> serves `index.html` at the subdirectory root by default, and the
> parent's in-surface links already expect that path.

## Embedded media

Tier II trailers embed their media inline as base64-encoded H.264 video
directly inside `index.html`, keeping each trailer single-file and
portable. The Bonded trailer's architecture animation is embedded this
way inside `/echo.bonded/index.html` — no sibling media file, no
external dependency, no separate asset to gate. This is the canonical
pattern for future `/echo.X/` trailers.

## License & use

This repository is published under
[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).
See `LICENSE` for full terms.

**You may:** read, link to, cite ECCO's amplification methodology and
the editorial framing, and share for non-commercial purposes with
attribution to Ethereal Connections Co.

**You may not:** repackage, rebrand, fork-and-resell, incorporate into
paid products, paid courses, paid newsletters, or any commercial
offering without prior written permission.

**You also may not** reproduce, excerpt, or redistribute any amplified
subject's underlying work — for the Bonded subject specifically, the
architecture itself, the embedded architecture animation, the five
Zenodo publications, or any content derived from US19438644 — without
separate written permission from that subject's originator. The
amplification framing, the editorial commentary, and the design system
are ECCO's; the underlying invention, research, art, animation, or
other representation of each subject's work is theirs. *Provenance
stays with the originator.*

As a surface default, an ECCO amplification is unsolicited editorial
commentary unless the subject's collaboration is explicitly named. For
the Bonded subject, the collaboration is named: the amplification is
published with Derek Antoine Lee's consent, under a service
arrangement in which ECCO designed, builds, and hosts his Tier III
surface. If any subject requests modification or removal of their ECCO
amplification, that request will be honored.

ECCO operates this repository under a public amplification posture.
Other ECCO surfaces (commercial methodology, revenue infrastructure)
are intentionally closed. The visibility of this repository is
amplification, not an invitation to extraction.

For commercial licensing, partnership, or any use beyond the terms above:
**jeremiah@etherealconnectionsco.com**

For permission to use Derek's underlying Bonded Science materials:
contact Derek directly via
[@derekantoinelee](https://instagram.com/derekantoinelee), or visit
his Tier III substance surface at
`bonded.etherealconnectionsco.com`. Each additional subject's
underlying work is governed by the same principle: contact the
originator directly.

## Doctrinal artifacts in play

This repo joins `scan-ecco`, `toolkit-ecco`, `mirror-ecco`, and
`echo-ecco` (all public, CC BY-NC-ND 4.0) on the public-surface side,
and `commission-ecco` (private, all rights reserved) on the
closed-methodology side. The build pipeline is the same on every
surface; what differs is the visibility posture and the surface-specific
integrity profile.

Amplification is a new surface category — distinct from diagnostic
(Scanner), educational (Toolkit), case-study (Mirror), and field-note
(Echo) surfaces. Amplification surfaces are multi-subject builder
showcases with the Provenance Echo doctrine made explicit: *the
architecture stays attributable to its originator*. The pattern is
parent surface + per-subject Tier II trailer (`/echo.X/`) +
per-subject Tier III substance at the originator's own domain. The
Mirror surface (`mirror.etherealconnectionsco.com/jowi/`) is the
structural precedent for the parent-plus-subdirectory layout. Bonded
is the first amplified subject on this surface; the lineage is
intended to grow as ECCO amplifies further builders whose work meets
the criteria.

---

*Part of the ECCO Transparency Project · Amplification lineage.*

*Provenance over performance. Infrastructure over influence. Doctrine over excuse.*
