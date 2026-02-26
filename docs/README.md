# SocialFlow Documentation

Official documentation for the SocialFlow platform.

## Features

- ✅ Full documentation website with VitePress
- ✅ Local search functionality
- ✅ Version selector
- ✅ Syntax highlighting for code examples
- ✅ Automated deployment

## Development

```bash
cd docs
npm install
npm run docs:dev
```

Visit `http://localhost:5173`

## Build

```bash
npm run docs:build
```

## Deployment

Documentation is automatically deployed via GitHub Actions to GitHub Pages when changes are pushed to `main` or `develop` branches.

### Manual Deployment

#### Vercel
```bash
vercel --prod
```

#### Netlify
```bash
netlify deploy --prod --dir=docs/.vitepress/dist
```

## Structure

```
docs/
├── .vitepress/
│   ├── config.ts          # VitePress configuration
│   └── theme/             # Custom theme
├── guide/                 # User guides
├── api/                   # API reference
├── examples/              # Code examples
├── versions/              # Version docs
└── index.md              # Homepage
```

## Contributing

1. Edit markdown files in `docs/`
2. Test locally with `npm run docs:dev`
3. Submit PR against `develop` branch
