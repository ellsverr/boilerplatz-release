# Boilerplatz Releases

This repository hosts encrypted release distributions for the Boilerplatz After Effects plugin.

## Structure

```
releases/
├── 0.3.0/
│   └── dist.zip (encrypted)
├── 0.4.0/
│   └── dist.zip (encrypted)
└── 0.5.0/
    └── dist.zip (encrypted)
```

## Security

- All release files are AES-256 encrypted with password protection
- Passwords are managed separately via Google Sheets (encrypted)
- Only authorized team members can decrypt and install releases

## Access

Releases are fetched automatically by the Boilerplatz plugin update system.

### Release URLs

Releases are accessible via GitHub Pages:
```
https://ellsverr.github.io/boilerplatz-release/releases/{version}/dist.zip
```

## Usage

This repository is managed by the automated release system. Do not manually upload files here unless you know what you're doing.

For creating releases, use the main Boilerplatz repository:
```bash
npm run release:patch
npm run release:minor
npm run release:major
```

---

**Note:** This is an internal distribution repository for the Boilerplatz team.

