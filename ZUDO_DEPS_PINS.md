# ZUDO_DEPS_PINS

Provenance for artifacts vendored or generated from first-party (takazudo/zudolab) upstreams.
Updated by /dev-bump-zudo-deps on every sync — keep `pinned:` accurate.

## create-zudo-doc scaffold
- repo: zudolab/zudo-doc
- what: generated doc-site scaffold, selectively customized and drift-gated
- files: pages/docs/[[...slug]].tsx, pages/index.tsx, pages/[locale]/docs/[[...slug]].tsx, public/favicon-16x16.png, public/favicon-32x32.png, public/favicon.ico, public/favicon.svg, scripts/check-links.js, scripts/setup-doc-skill.sh, src/styles/global.css, tsconfig.json
- source: packages/create-zudo-doc/templates/base/ -> repo root; packages/create-zudo-doc/templates/features/i18n/files/ -> repo root
- track: releases
- pinned: 82049856397927077c5288465db34e44d0939260 (v7.0.0; published create-zudo-doc@7.0.0)
- updated: 2026-10-15
- notes: Compared every published 7.0.0 base/i18n template byte against this host, including all manifest files. Adopted the explicitly relative tsconfig path alias and removed baseUrl. Route stubs retain the generator's DocHistoryBoundary feature binding; global.css retains Noto/Futura branding and now sets the supported header-logo font/weight tokens. These are the only allowlisted template differences; all other base/i18n files, including setup-doc-skill.sh, check-links.js and favicons, match 7.0.0. Preserve short codemirror-wisdom package-script arguments, explicit branding/localized navigation, dark default, dynamicPageTransition:false, CodeMirror IIFE build and HtmlPreview asset injection. Typecheck, template drift, pin parity and Wrangler parity passed on Node 24; the complete ten-step b4push gate also passed with 92 pages built. Rendered UI validation is coordinated separately and is not claimed here.
