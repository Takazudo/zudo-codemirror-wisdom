# ZUDO_DEPS_PINS

Provenance for artifacts vendored or generated from first-party (takazudo/zudolab) upstreams.
Updated by /dev-bump-zudo-deps on every sync — keep `pinned:` accurate.

## create-zudo-doc scaffold
- repo: zudolab/zudo-doc
- what: generated doc-site scaffold, selectively customized and drift-gated
- files: pages/docs/[[...slug]].tsx, pages/index.tsx, pages/[locale]/docs/[[...slug]].tsx, public/favicon-16x16.png, public/favicon-32x32.png, public/favicon.ico, public/favicon.svg, scripts/check-links.js, scripts/setup-doc-skill.sh, src/styles/global.css, tsconfig.json
- source: packages/create-zudo-doc/templates/base/ -> repo root; packages/create-zudo-doc/templates/features/i18n/files/ -> repo root
- track: releases
- pinned: 70c574747e498c47f35fa9051ab36b0a69ac808d (v10.0.0; published create-zudo-doc@10.0.0)
- updated: 2026-11-10
- notes: Diffed published 10.0.0 base/i18n templates against 7.0.0. Only scripts/setup-doc-skill.sh changed; it was recopied verbatim (worktree porcelain, one locale-presence decision, AUTHORING placement step). Allowlisted diffs stay the DocHistoryBoundary route stubs and global.css Noto/Futura branding (header-logo font/weight tokens). Every other listed file matches 10.0.0. Preserve short codemirror-wisdom package-script arguments, branding, localized navigation, dark default, omitted themePack (zudo-doc 10 resolves that to Graphite; do not pin classic or list default with graphite), dynamicPageTransition:false, the CodeMirror IIFE build, and HtmlPreview asset injection. Do not add a direct @takazudo/zdtp pin while designTokenPanel is off. Keep wrangler exact at the version embedded in the installed zfb binary. Node 24 verification: the ten b4push steps passed individually and the build wrote 92 pages.
