# Blog-First Site Configuration

Your Hugo site is now configured so that `/blog` is the main landing page and the primary URL structure.

## What's Been Set Up

1. **Homepage Redirect**: `zoraizanwar.me/` automatically redirects to `zoraizanwar.me/blog/`
2. **Blog as Main Section**: The blog section is configured as the main content area
3. **URL Structure**: All blog posts appear under `/blog/` with clean URLs
4. **Navigation**: The "Blog" menu item points to `/blog` and will be highlighted when active

## Current Structure

```
content/
├── _index.md                    # Root page (redirects to /blog)
├── blog/                        # Main blog section
│   ├── _index.md               # Blog listing page (/blog)
│   ├── exploring-new-tech/     # Blog post (/blog/exploring-new-tech/)
│   ├── first-post/             # Blog post (/blog/first-post/)
│   └── travel-adventures/      # Blog post (/blog/travel-adventures/)
├── about.md                    # About page (/about)
└── docs/                       # Documentation section (/docs)
```

## Configuration Changes

1. **hugo.yaml**: 
   - Added `mainSections: ["blog"]`
   - Added `permalinks` for blog posts
   - Updated menu to point to `/blog`

2. **layouts/index.html**: 
   - Homepage redirects to `/blog/`

3. **content/blog/_index.md**: 
   - Main blog page with introduction

## URL Behavior

- `zoraizanwar.me/` → redirects to `zoraizanwar.me/blog/`
- `zoraizanwar.me/blog/` → main blog listing page
- `zoraizanwar.me/blog/post-name/` → individual blog posts
- Blog menu item highlights when on `/blog/` or any blog post

This setup ensures that your blog is always the primary focus and the default landing experience for visitors.
