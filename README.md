# Decisional Documentation

Official documentation for [Decisional](https://www.decisional.com) - the spreadsheet-native automation platform.

## What's Included

- **Getting Started** - Quickstart, core concepts, and setup
- **User Guides** - Comprehensive guides for agents, worksheets, sources, AI assistant, runs, integrations, and workspaces
- **Reference** - Glossary, FAQ, and changelog
- **Branding** - Custom Decisional purple theme (#3E0D77)

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview documentation changes locally:

```bash
npm i -g mintlify
```

Run the following command at the root of your documentation (where mint.json is):

```bash
mintlify dev
```

The docs will be available at `http://localhost:3000`

## Publishing Changes

Changes are automatically deployed to production when pushed to the `main` branch via Mintlify's GitHub integration.

**Workflow:**
1. Make changes to .mdx files or mint.json
2. Commit and push to `main`
3. Mintlify automatically deploys updates

## Documentation Structure

```
├── introduction.mdx          # Homepage
├── quickstart.mdx            # 5-minute getting started guide
├── core-concepts.mdx         # Deep dive into platform concepts
├── setup.mdx                 # Account and workspace setup
├── guides/
│   ├── agents.mdx            # Working with agents
│   ├── worksheets.mdx        # Spreadsheet operations
│   ├── sources.mdx           # Document processing and RAG
│   ├── ai-assistant.mdx      # Interactive testing
│   ├── runs.mdx              # Monitoring and debugging
│   ├── integrations.mdx      # Connecting external services
│   └── workspaces.mdx        # Team collaboration
└── reference/
    ├── glossary.mdx          # Key terms
    ├── faq.mdx               # Common questions
    └── changelog.mdx         # Product updates
```

## Troubleshooting

- **Mintlify dev isn't running** - Run `mintlify install` to re-install dependencies
- **Page loads as a 404** - Make sure you are running in a folder with `mint.json`
- **Changes not appearing** - Clear browser cache or hard refresh (Cmd+Shift+R / Ctrl+Shift+F5)

## Links

- **Documentation**: https://docs.decisional.com
- **App**: https://agents.decisional.com
- **Website**: https://www.decisional.com
- **Blog**: https://www.decisional.com/blog
- **Discord**: https://discord.gg/DwPDS5Prk2
