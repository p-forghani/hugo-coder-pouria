# Static Assets

This directory contains static assets for your Hugo website.

## Required Files

Based on your `hugo.toml` configuration, you need to add the
following files:

### Avatar/Profile Picture
- **Location:** `static/images/avatar.jpg`
- **Description:** Your profile picture that appears on the homepage
- **Recommended size:** 400x400px or larger (square format)
- **Format:** JPG, PNG, or WebP

### Favicons
These appear in browser tabs and bookmarks:

- **Location:** `static/img/favicon.svg`
  - Vector favicon (modern browsers)
  - Can be created from a PNG using online tools

- **Location:** `static/img/favicon-32x32.png`
  - 32x32 pixel favicon
  
- **Location:** `static/img/favicon-16x16.png`
  - 16x16 pixel favicon

## How to Add Files

1. **Avatar**: Place your profile photo at
   `static/images/avatar.jpg`

2. **Favicons**: You can generate all favicon sizes from a single
   image using online tools like:
   - https://realfavicongenerator.net/
   - https://favicon.io/

   Then place the generated files in `static/img/`

## Alternative: Use Gravatar

If you don't want to add a local avatar, you can uncomment line 25 in
`hugo.toml`:
```toml
gravatar = "forghani.dev@gmail.com"
```

This will use your Gravatar image instead of a local file.

## Directory Structure

```
static/
├── images/
│   └── avatar.jpg          (your profile picture)
└── img/
    ├── favicon.svg         (vector favicon)
    ├── favicon-32x32.png   (32x32 favicon)
    └── favicon-16x16.png   (16x16 favicon)
```
