---
layout: layouts/post.njk
title: My first post
description: The first post on the Eleventy + Netlify CMS from scratch blog
date: 2020-10-08
featuredImage: /images/uploads/image1.png
tags: ["cat", "dog"]
---
## tags

Trying to understand the way the `posts` folder is processed from input to output. 

The `posts.json` file seems to be adding `"tags: posts"` to every post so that a collection of "tags: posts" can be used to create a list of posts.

This was confirmed by adding displays of front matter to each post, using the layout post.njk.

`tags`, as well as `date`, are now displayed when a post in the post list is clicked.

Other front matter can also be shown... [TODO]

How to create a list of clickable unique tags... [TODO]

But, when adding tags to the front matter directly, the `posts` tag no longer appeared, and the post was absent from the posts list.

## searching

Just to note that this search was successful, and the results are understandable. 

[Merge tags when defined in multiple places](https://github.com/11ty/eleventy/issues/401)

[QUICK TIP #004—ZERO MAINTENANCE TAG PAGES FOR YOUR BLOG](https://www.11ty.dev/docs/quicktips/tag-pages/)

[Data Deep Merge](https://www.11ty.dev/docs/config/#data-deep-merge)

[Using data | Data cascade | data deep merge](https://www.11ty.dev/docs/data-deep-merge/)

[Frontmatter properties replace those in .json files rather than supplementing](https://github.com/11ty/eleventy/issues/147)

## Solving the problem

The `dot eleventy dot js` file was updated with the configuration change and the tags are now merged. Need to look out for when this approach is part of the mainline and the config change is not needed.

## in passing

[eleventy tips](https://11tytips.netlify.app/)

[importing json using curl](https://github.com/11ty/eleventy-community/issues/4#issuecomment-597866277)

[more on eleventy data](https://www.11ty.dev/docs/data-global/)

[Collection of tags](https://github.com/11ty/eleventy/issues/927)

[Collections (using tags)](https://www.11ty.dev/docs/collections/)

##  netlify status

[Netlify status badge for success, building or failed](https://app.netlify.com/sites/fomf-22/settings/general#status-badges)

[![Netlify Status](https://api.netlify.com/api/v1/badges/5b4f71ff-b884-40ac-b4f0-d4067c1f8067/deploy-status)](https://app.netlify.com/sites/fomf-22/deploys)