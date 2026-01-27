# Decisional Public Documentation

This is the Mintlify-powered documentation for Decisional, hosted at `docs.decisional.com`.

## Structure

```
decisional-docs/
├── mint.json           # Navigation, theme, and config
├── introduction.mdx    # Landing page
├── quickstart.mdx      # Getting started guide
├── guides/             # Feature guides (create as needed)
├── integrations/       # Integration setup guides (create as needed)
├── api-reference/      # API documentation
├── images/             # Screenshots and GIFs
│   ├── guides/
│   └── integrations/
└── snippets/           # Reusable content blocks
```

## Common Commands

```bash
# Install Mintlify CLI
npm i -g mintlify

# Run local dev server
mintlify dev

# Check for broken links
mintlify broken-links
```

## Adding a New Page

1. Create `.mdx` file in appropriate folder
2. Add to `mint.json` navigation
3. Add images to `images/` folder

## MDX Page Template

```mdx
---
title: 'Page Title'
description: 'Brief description for SEO and previews'
icon: 'icon-name'  # Optional FontAwesome icon
---

## Overview

Introduction paragraph.

## Section

Content with images:

<img src="/images/guides/example.png" alt="Description" />

### Subsection

More content.

<Tip>
  Highlight important information with callouts.
</Tip>

<Warning>
  Warn users about potential issues.
</Warning>
```

## Navigation (mint.json)

To add pages to the sidebar, edit the `navigation` array in `mint.json`:

```json
{
  "group": "Guides",
  "pages": [
    "guides/scheduling",
    "guides/integrations"
  ]
}
```

## Image Guidelines

- **Location**: `images/{section}/{feature-name}.png`
- **Format**: PNG for screenshots, GIF for animations
- **Size**: Max width 1200px, optimize for web
- **Alt text**: Always include descriptive alt text

## URL Structure

Pages map to URLs:
- `guides/scheduling.mdx` → `docs.decisional.com/guides/scheduling`
- `integrations/slack.mdx` → `docs.decisional.com/integrations/slack`

## Writing Style

- **Customer-focused**: Explain benefits, not just features
- **Action-oriented**: Start with what users can DO
- **Concise**: Get to the point quickly
- **Visual**: Include screenshots for UI steps
- **Structured**: Use consistent heading hierarchy
