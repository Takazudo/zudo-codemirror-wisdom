# ZUDO_DEPS_PINS

Provenance for artifacts vendored or generated from first-party (takazudo/zudolab) upstreams.
Updated by /dev-bump-zudo-deps on every sync — keep `pinned:` accurate.

## create-zudo-doc scaffold
- repo: zudolab/zudo-doc
- what: generated doc-site scaffold, selectively customized and drift-gated
- files: pages/docs/[[...slug]].tsx, pages/index.tsx, pages/[locale]/docs/[[...slug]].tsx, public/favicon-16x16.png, public/favicon-32x32.png, public/favicon.ico, public/favicon.svg, scripts/check-links.js, scripts/setup-doc-skill.sh, src/styles/global.css, tsconfig.json
- source: packages/create-zudo-doc/templates/base/ -> repo root; packages/create-zudo-doc/templates/features/i18n/files/ -> repo root
- track: releases
- pinned: b4f974598b27064a092eeadb5b2e5559078a8bb9 (v6.0.0)
- updated: 2026-10-11
- notes: Reconciled published create-zudo-doc 5.28.1 → 6.0.0. Adopted zudo-react JSX types and the docHistory transformer’s DocHistoryBoundary binding in both host route stubs, removed Preact aliases from tsconfig, and migrated CSS to zudo-wind layers/plain :root tokens while preserving Noto Sans JP/Futura branding. The logo selector is a[data-header-logo] so authored normal weight wins over generated utilities. All other tracked base/i18n scaffold files are unchanged upstream; check-links.js and setup-doc-skill.sh were compared byte-for-byte between releases. setup-doc-skill.sh remains the stock 6.0.0 template, unchanged since 5.28.1. Preserve the short codemirror-wisdom package-script arguments and header navigation. Full b4push passed, including the non-allowlisted template drift gate. Chromium verified repeated navigation, search/appearance controls, Japanese routes and the mobile sidebar with no page errors.
