---
title: Creating docs and frontmatter
---
This is an example doc. Docs are Markdown files inside the `content/` directory.

***

## Creating new docs

Creating a new knowledge base doc is easy:

1. Using Obsidian, Visual Studio Code, iA Writer, any text editor, or via your computer's operating system file manager, create a new file with any name and ending with the `.md` file extension.
2. If this new file was created in the `content/` directory, then it is now a part of your knowledge base docs.

***

## Frontmatter / properties in docs

Because docs are Markdown files, you can include metadata at the top of them using YAML frontmatter.

This metadata is added as YAML frontmatter and placed between a pair of triple-dashed lines (an upper `---` and a lower `---`).

> [!CAUTION]
>
> 1. YAML frontmatter MUST be the first thing in a Markdown file.
> 2. YAML frontmatter MUST be placed between triple-dashed lines (`---`).
>
> [!TIP] Obsidian calls frontmatter `Properties`
>
> *If you use Obsidian to edit your Markdown docs, YAML frontmatter is referred to as `Properties` or `File properties`*.

The knowledge base docs website is powered by [Quartz](https://quartz.jzhao.xyz/), a static-site generator for turning Markdown docs into websites.

#### Common frontmatter fields

These are the most common frontmatter fields:

- `title`: Title of the page. If not provided, Quartz will use the filename.
- `description`: Description of the page used for link previews.
- `permalink`: A custom URL for the page that will remain constant even if the path to the file changes.
- `aliases`: Other names for this note (list of strings).
- `tags`: Tags for this note.
- `draft`: Whether to publish the page or not.
- `date`: The published date, normally `YYYY-MM-DD`.

(list via [the Quartz docs](https://github.com/jackyzha0/quartz/blob/v4/docs/authoring%20content.md))

#### Full list of supported frontmatter fields

Quartz supports these (canonical names shown; Quartz also recognizes many aliases):

- title
- description
- permalink
- comments
- lang
- publish
- draft
- enableToc
- tags / tag
- aliases / alias
- cssclasses / cssclass
- socialDescription
- socialImage / image / cover
- created / date
- modified / lastmod / updated / last-modified
- published / publishDate / date

(list via [the Quartz docs](https://github.com/jackyzha0/quartz/blob/v4/docs/plugins/Frontmatter.md))

---

Example YAML frontmatter you can copy:

```yaml
---
title: "Creating docs and frontmatter"
description: "How to write docs and use YAML frontmatter for the site"
date: 2026-08-24
tags:
  - docs
  - frontmatter
draft: false
permalink: /docs/creating-docs-and-frontmatter/
---
```

## Markdown references

Here are some helpful references for the type of Markdown you can use in your knowledge base docs:

- [Basic formatting syntax](https://help.obsidian.md/syntax)
- [Obsidian Flavored Markdown](https://help.obsidian.md/obsidian-flavored-markdown)
- [GitHub Flavored Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
