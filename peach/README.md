# Peach Theme (Help Center)

Example Help Center site using the Peach theme.

## Structure

```
├── index.mdx                     # Homepage (hero + search + group tiles)
├── getting-started/
│   ├── index.mdx                 # Directory page (frontmatter-only)
│   ├── quick-setup.mdx           # Article
│   ├── first-project.mdx         # Article
│   └── invite-team.mdx           # Article
├── billing/
│   ├── index.mdx                 # Directory page
│   ├── change-plan.mdx           # Article
│   ├── invoices.mdx              # Article
│   └── payment/
│       ├── index.mdx             # Sub-category directory page
│       ├── add-card.mdx          # Article
│       └── bank-transfer.mdx     # Article
├── integrations/
│   ├── index.mdx                 # Directory page
│   ├── slack.mdx                 # Article
│   └── github.mdx                # Article
└── docs.json
```

## Key differences from docs themes

- `root` is **required** on every group (every category is visitable)
- Directory pages (group root pages with empty body) auto-render a `<PageList />` of children
- If a root page has content, the directory listing is shown alongside it (like API playground pages)
- `description` and `image` for categories come from the root page's **frontmatter**, not `docs.json`
- Breadcrumbs default to on (`styling.eyebrows: "breadcrumbs"`)
- Navigation is tile/list-based instead of sidebar
