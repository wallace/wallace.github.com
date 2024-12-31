# Two Minute Spates Blog

Personal blog built with Jekyll and the Hyde theme. Visit at [blog.jonathanrwallace.com](https://blog.jonathanrwallace.com).

## Setup

1. Install dependencies:
``` bash
    bundle install
```

2. Run the development server:
```bash
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`

## Creating New Posts

1. Create a new post in the `_posts` directory with the format:
```bash
YEAR-MONTH-DAY-title.markdown
```

For example:
```bash
2024-01-15-my-new-post.markdown
```

2. Add the front matter to your post:
```
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD HH:MM:SS -0500
categories: [optional-categories]
---

Your post content here...

<!-- more -->

Rest of your post...
```

The `<!-- more -->` tag determines what shows on the home page as an excerpt.

## Development

- Posts are in `_posts/`
- Pages are in the root directory (e.g., `about.html`, `archive.html`)
- Layouts are in `_layouts/`
- Includes (reusable components) are in `_includes/`
- CSS is in `public/css/`

## Theme

Using the Hyde theme with customizations:
- Blue color scheme (`theme-base-0d`)
- Custom sidebar styling
- Modified layout for posts and pages

## Deployment

The site is automatically deployed via GitHub Pages when changes are pushed to the main branch.

## Local Development Commands

### Start the development server
``` bash
bundle exec jekyll serve
```

### Start with drafts enabled
``` bash
bundle exec jekyll serve --drafts
```

### Build the site
``` bash
bundle exec jekyll build
```

### Create a new post (replace TITLE)
``` bash
bundle exec jekyll post "TITLE"
```

## Writing Tips

1. Use front matter for post metadata:
```yaml
---
layout: post
title: "Your Title"
date: YYYY-MM-DD HH:MM:SS -0500
categories: [category1, category2]
tags: [tag1, tag2]
---
```

2. Add images:
```markdown
![Alt text](/path/to/image.jpg)
```

3. Add code blocks:
````markdown
```ruby
def hello
  puts "Hello, World!"
end
```
````

4. Add links:
```markdown
[Link text](URL)
```

## Directory Structure

```
.
├── _config.yml
├── _includes/
├── _layouts/
├── _posts/
├── public/
│   └── css/
├── index.html
├── about.html
├── archive.html
└── README.md
```

## Configuration

Main configuration is in `_config.yml`. Key settings:
- Site title and description
- Theme settings
- Build settings
- Plugin configuration

## License

Content is copyrighted by Jonathan R Wallace. Theme is MIT licensed.