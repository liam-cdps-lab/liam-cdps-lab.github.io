[<< Back to documentation index](./README.md)

# Create a new post

When you create a new post you should create both an English and Welsh version.

Create a file for the English version in `en/updates/_posts`.

Create a file for the Welsh version in `cy/updates/_posts`.

The files should be markdown files (end with `.md` extension).

And follow the format `YYYY-MM-DD-name-of-post.md`. The filename is used to create the URL. It will automatically convert to `you-site-url/en/updates/YYYY/MM/DD/name-of-post.html` with `en` replace by `cy` for the Welsh version.

Once you've created the files they will appear on the respective `/<lang>/updates/` page.

## What to put in the file

The contents of a file will look something like this

```
---
title: Sample update
layout: post
lang: en
ref: sample-update
author: Template bot
---

The post content...
```

All post files start with some metadata - this is called frontmatter. It is used to provide some information about the post you are about to write. For example, you might use it to add the author. The project site template will also use it to link together the different language versions of a post.

The content of the post must follow the metadata.

The key attributes to note are `lang` and `ref`. `lang` should be set to `en` or `cy` depending on the language of the post. Set `ref` to whatever like, we keep it similar to the post title for simplicity, but make sure you use the same value for both versions of the post. This is the value that is used to link the different versions together. If these don't match then the link between the different versions will not work.

