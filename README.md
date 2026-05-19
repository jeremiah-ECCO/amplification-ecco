# echo.bonded — Bonded Tier II Trailer

The **Bonded Tier II trailer** of the ECCO Amplification Surface — the
ECCO-authored editorial trailer for the Bonded Science work of
**Derek Antoine Lee** (`@treeminded` / `@derekantoinelee`). Deployed as a
subdirectory at `amplification.etherealconnectionsco.com/echo.bonded/`,
beneath the Tier I parent surface.

Tier III substance — Derek's own surface — is live and independent at
`bonded.etherealconnectionsco.com`. *Provenance preserved. Originator-held.*

## What this is

A single self-contained immersive trailer (gate, then scenes) that
introduces Derek's Bonded Science framework and forwards visitors to his
Tier III surface. The architecture animation is embedded inline as
H.264-encoded base64 video, keeping the trailer a portable single file.

## Posture — named collaboration

This amplification is published **with Derek Antoine Lee's consent**, as
the editorial layer of an ongoing collaboration. ECCO designed, built, and
hosts Derek's Tier III surface (`bonded.etherealconnectionsco.com`) under a
**service arrangement** with him; this trailer is part of that same
collaboration. It is **not** an unsolicited amplification — the
collaboration is named here and on the surface itself.

(The Amplification Surface's general posture treats an amplification as
unsolicited *unless* the subject's collaboration is explicitly named. For
Bonded, it is named: this is a consented collaboration.)

## Rights

The editorial layer — the trailer's framing, copy, design system, and
doctrinal commentary — is ECCO's, licensed under
[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).
See `LICENSE`.

**The embedded architecture animation is NOT part of that grant.** The
animation is a representation of Derek's Bonded Science framework. Per the
service arrangement, and consistent with Derek's own Tier III `LICENSE`,
**ECCO holds no rights to the Bonded Science framework, its
representations, the patent filing, the Zenodo deposits, the architecture,
the diagrams, or the animation.** All rights and distribution rights in
Derek's underlying work — including the embedded animation — are reserved
to **Derek Antoine Lee**. Bonded Science is listed **Private for Study**.

## Build gate

```
node check-links.mjs index.html 404.html
```

Runs on Netlify Node 20, no local install required. `check-links.mjs` is
the universal ECCO v4 link-integrity gate — a dead external link fails the
build before it can ship.

> **Kit status.** While this trailer is nested under the Tier I parent
> surface, the parent's `netlify.toml` governs the build and the parent's
> `404.html` serves as the error page. The files in this kit
> (`netlify.toml`, `404.html`, `check-links.mjs`, `LICENSE`, `README.md`,
> `.gitignore`) are inactive carry-along artifacts — maintained so the
> trailer can be extracted to its own subdomain cleanly if that is ever
> needed.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The Bonded Tier II trailer — single self-contained immersive; animation embedded as base64 H.264 video |
| `404.html` | Custom 404 |
| `check-links.mjs` | Universal ECCO v4 build-gate link checker |
| `netlify.toml` | Build configuration (governs only on standalone extraction) |
| `LICENSE` | CC BY-NC-ND 4.0 on ECCO's editorial layer, with the Bonded work — including the embedded animation — carved out to Derek Antoine Lee |
| `.gitignore` | Standard exclusions |

## Inquiries

For the Bonded Science framework, licensing, collaboration, or any use
beyond private study — **direct correspondence to Derek Antoine Lee**
(`@derekantoinelee`), or visit `bonded.etherealconnectionsco.com`. ECCO
does not accept or route inquiries about the underlying work.

For ECCO's editorial methodology or the Amplification Surface:
**jeremiah@etherealconnectionsco.com**

---

*Part of the ECCO Transparency Project · Amplification lineage.*

*Provenance over performance. Infrastructure over influence. Doctrine over excuse.*
