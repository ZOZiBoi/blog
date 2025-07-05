# Page Bundles for Blog Posts

This blog uses Hugo's **page bundles** feature, which allows each blog post to have its own folder containing the post content and all associated assets (images, documents, etc.).

## Structure

Each blog post should be organized as follows:

```
content/blog/
├── my-post-name/
│   ├── index.md          # The main post content
│   ├── featured-image.jpg # Featured image
│   ├── diagram.png       # Post images
│   ├── document.pdf      # Other assets
│   └── ...               # Any other files
└── another-post/
    ├── index.md
    └── ...
```

## Creating a New Post

### Method 1: Using Hugo CLI
```bash
hugo new content/blog/my-new-post/index.md
```

This will create a new folder `my-new-post/` with an `index.md` file using the archetype template.

### Method 2: Manual Creation
1. Create a new folder in `content/blog/` with your post name
2. Create an `index.md` file inside that folder
3. Add your post content and frontmatter

## Including Images and Assets

Since all assets are in the same folder as your post, you can reference them with simple relative paths:

```markdown
![Alt text](my-image.jpg)
![](my-image.jpg)  # No alt text

<!-- For custom sizing, use HTML img tags -->
<img src="my-image.jpg" alt="Alt text" width="400">
<img src="my-image.jpg" alt="Alt text" style="max-width: 400px;">
```

## Benefits of Page Bundles

1. **Organization**: Each post is self-contained with all its assets
2. **Portability**: Easy to move posts between sites
3. **No broken links**: Images are bundled with the post
4. **Clean URLs**: Posts get clean URLs like `/blog/my-post-name/`
5. **Asset processing**: Hugo can optimize images in the same folder

## Example Post Structure

```markdown
---
title: "My Amazing Post"
slug: "my-amazing-post"
description: "A description of my post"
tags: ["hugo", "blog"]
date: 2025-01-15
draft: false
image: "featured-image.jpg"  # Featured image from this folder
---

# My Amazing Post

Here's some content with an image:

![My screenshot](screenshot.png)

Here's an image with custom sizing:

<img src="screenshot.png" alt="My screenshot" width="600">

And here's a document: [Download PDF](document.pdf)
```

## Tips

- Keep image file names descriptive and web-friendly
- Use lowercase filenames with hyphens instead of spaces
- Optimize images before adding them to your post folder
- The `image:` frontmatter field should reference the featured image filename
- Set `draft: false` when ready to publish
