# PRD — MiniDev Landing Page

## Problem Statement (original)
Landing page resmi statis untuk aplikasi Windows "MiniDev" (Beta v0.1.0): dark premium theme, hero, product intro, features, why-compare, specs, documentation, runtime storage guide, beta notice, requirements, FAQ, download CTA (external Google Drive URL via config), SEO/OpenGraph. Tanpa backend, tanpa DB, tanpa auth, tanpa GitHub/repo mentions.

## Architecture
- Frontend-only SPA: React + custom CSS (Tailwind/craco build).
- /app/frontend/src/App.js — seluruh section landing page.
- /app/frontend/src/App.css — dark/glass theme styling.
- /app/frontend/public/index.html — SEO, OpenGraph, favicon.
- Backend & MongoDB: tidak digunakan (by design).

## User Personas
- Developer PHP/Laravel Windows yang ingin local dev environment ringan.

## Implemented
- 2026-09: Base landing page lengkap (Navbar sticky, Hero, Intro, Features, Why MiniDev, Specs, Docs, Runtime Storage, Beta Notice, Requirements, FAQ, Download, Footer).
- 2026-09: DOWNLOAD_URL config → Google Drive link asli.
- 2026-09: Logo, screenshots, favicon, social-preview metadata.
- 2026-09: Release notes & visual runtime guide.
- 2026-09: E2E frontend test passed (iteration_1/3/4/5 reports).

## Backlog
- P0: Tidak ada.
- P1: Revisi copy/layout jika user memberi feedback.
- P2: Refactor App.js ke komponen modular jika situs diperluas.

## Next Tasks
- Menunggu feedback user (GitHub push via tombol "Save to Github" di UI Emergent).
