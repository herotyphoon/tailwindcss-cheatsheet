# Contributing to Tailwind CSS Cheatsheet

Thank you for your interest in contributing! This is a community resource and every improvement helps developers around the world. 🎉

---

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Making Changes](#making-changes)
- [Pull Request Process](#pull-request-process)
- [Style Guide](#style-guide)

---

## Code of Conduct

Please read and follow our [Code of Conduct](CODE_OF_CONDUCT.md). We expect all contributors to uphold it.

---

## How Can I Contribute?

### 🐛 Reporting Bugs / Missing Utilities

If you find a missing class, incorrect CSS value, or a broken layout:

1. **Search existing issues** first to avoid duplicates
2. Open a new issue using the **Bug Report** template
3. Include the class name, what it should do, and what it currently shows (or doesn't)

### ✨ Suggesting Enhancements

Have an idea for a new section or improvement?

1. Open an issue using the **Feature Request** template
2. Describe what you want and why it would be useful
3. Wait for a maintainer to approve before working on it (to avoid wasted effort)

### 📝 Improving Documentation

Small fixes like typos, clarity improvements, or better examples are always welcome — no issue needed for minor changes.

---

## Getting Started

```bash
# 1. Fork the repo on GitHub, then clone your fork
git clone https://github.com/YOUR_USERNAME/tailwind-cheatsheet.git
cd tailwind-cheatsheet

# 2. Open index.html in your browser
open index.html

# 3. Create a feature branch
git checkout -b fix/missing-backdrop-utilities
# or
git checkout -b feat/add-tailwind-v4-section
```

---

## Making Changes

The entire cheatsheet lives in **`index.html`** — it is intentionally a single file with no build step.

### Structure of `index.html`

- **`<style>`** — All CSS variables and component styles are at the top
- **`<nav>`** — Sticky navigation links. Add a link here if you add a new section
- **`<section>`** blocks — Each section has an `id` and a color theme class (`s-sky`, `s-violet`, etc.)
- **Table structure** — Use `.ref-table` with `.class-col`, `.val-col`, `.css-col` td classes

### Adding a New Utility Row

```html
<tr>
  <td class="class-col">new-utility-class</td>
  <td class="css-col">css-property: value</td>
</tr>
```

### Adding a New Section

```html
<section id="my-section" class="s-sky">  <!-- or s-violet, s-emerald, s-pink, s-orange -->
  <div class="section-title">🔷 My Section</div>
  <div class="grid-2">
    <div class="card">
      <div class="card-header">
        <span class="dot" style="background:var(--accent)"></span>Subsection Title
      </div>
      <table class="ref-table">
        <tr><th>Class</th><th>CSS</th></tr>
        <!-- rows here -->
      </table>
    </div>
  </div>
</section>
```

Don't forget to add a `<a href="#my-section">My Section</a>` link in the `<nav>`.

---

## Pull Request Process

1. **Keep PRs focused** — one topic per PR (don't mix a bug fix with a new feature)
2. **Update the CHANGELOG** — add an entry under `[Unreleased]`
3. **Test in multiple browsers** — Chrome, Firefox, and Safari if possible
4. **Screenshot your change** if it affects the visual layout
5. Submit the PR against the `main` branch

### PR Title Format

```
fix: add missing backdrop-saturate utilities
feat: add Tailwind v4 alpha changes section
docs: fix typo in README
chore: update color swatch for rose-950
```

### What Happens After You Submit

- A maintainer will review within a few days
- They may request changes or ask clarifying questions
- Once approved, your PR will be squash-merged and credited in the CHANGELOG

---

## Style Guide

### CSS / HTML

- Use the existing CSS variable system (`var(--accent)`, `var(--muted)`, etc.)
- Keep styles inside the `<style>` block at the top — no inline styles except for color swatches
- Use semantic HTML — `<table>` for tabular data, `<section>` for logical groupings

### Accuracy

- Double-check values against the [official Tailwind CSS docs](https://tailwindcss.com/docs)
- Include the exact CSS output, not just a description
- If a utility accepts a scale (like spacing), show the pattern with `{n}` notation

### Language

- Use clear, concise language
- American English spelling
- No fluff — this is a reference, not a tutorial

---

## Questions?

Open a [Discussion](https://github.com/YOUR_USERNAME/tailwind-cheatsheet/discussions) if you're unsure about anything. We're happy to help!
