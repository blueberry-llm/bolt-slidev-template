# Slidev Template

A starter template for [bolt.diy](https://github.com/stackblitz-labs/bolt.diy).

## Purpose

This template is designed for use with **<https://github.com/stackblitz-labs/bolt.diy>**. bolt.diy fetches
these files at runtime and imports them into a fresh WebContainer project when you ask for a Slidev presentation,
so everything here needs to install and build with no extra setup.

Modified by [Dustin Loring](https://github.com/Dustinwloring1988) (Dustinwloring1988) in October 2026.

## Stack

| Package | Version |
| --- | --- |
| @slidev/cli | ~52.14.0 |
| @slidev/theme-default | ^0.25.0 |
| @slidev/theme-seriph | ^0.25.0 |

## Commands

```bash
npm install   # install dependencies
npm run dev   # slidev — dev server
npm run build # slidev build — build presentation
npm run export # slidev export — export to static HTML
```

## About this template

A basic Slidev presentation with the default serif theme. Slidev 52.14.x is the last version that builds
without errors introduced by the lightningcss CSS parser. Newer Slidev 52.15.0+ changes a CSS property
(`margin-right:1.5rem;width:1rem`) that breaks lightningcss, so the version is pinned to ~52.14.0.

## Upgraded to Slidev ~52.14.0 (October 2026)

The template originally had `@slidev/cli` with a floating `latest` tag. This was replaced with the exact
pin `~52.14.0` (52.14.2) to avoid the known build failure on Slidev 52.15.0+. All other dependencies
(@slidev/theme-default, @slidev/theme-seriph) remain at their latest compatible ranges.

This pinning ensures `npm install` completes successfully and `slidev build` renders the presentation
without lightningcss errors.

## Verification

- `npm install` completes without errors
- `slidev build` produces a presentation bundle
- Confirmed the presentation renders in the browser without CSS parse errors