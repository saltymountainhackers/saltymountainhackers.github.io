---
layout: page
title: "contribute"
date: 2013-05-04 16:32
comments: true
sharing: true
footer: true
---

This community site is based on [Octopress](http://octopress.org/) a static site generator. It is
hosted on [Github](http://github.com) and is split into two branches

* [Source](https://github.com/saltymountainhackers/saltymountainhackers.github.io/tree/source) Contains
  the source markup.
* [Master](https://github.com/saltymountainhackers/saltymountainhackers.github.io) Contains the generated
  html markup.

To contribute you need to install ruby 1.9.3 and bundler. Checkout the source branch and then do

```
rake -T
```

and you will see a list of options

```
rake clean                     # Clean out caches: .pygments-cache, .gist-cache, .sass-cache
rake copydot[source,dest]      # copy dot files for deployment
rake deploy                    # Default deploy task
rake gen_deploy                # Generate website and deploy
rake generate                  # Generate jekyll site
rake install[theme]            # Initial setup for Octopress: copies the default theme into the path of Jekyll's generator.
rake integrate                 # Move all stashed posts back into the posts directory, ready for site generation.
rake isolate[filename]         # Move all other posts than the one currently being worked on to a temporary stash location (stash) so regenerating the site happens much more quickly.
rake list                      # list tasks
rake new_page[filename]        # Create a new page in source/(filename)/index.markdown
rake new_post[title]           # Begin a new post in source/_posts
rake preview                   # preview the site in a web browser
rake push                      # deploy public directory to github pages
rake rsync                     # Deploy website via rsync
rake set_root_dir[dir]         # Update configurations to support publishing to root or sub directory
rake setup_github_pages[repo]  # Set up _deploy folder and deploy branch for Github Pages deployment
rake update_source[theme]      # Move source to source.old, install source theme updates, replace source/_includes/navigation.html with source.old's navigation
rake update_style[theme]       # Move sass to sass.old, install sass theme updates, replace sass/custom with sass.old/custom
rake watch                     # Watch the site and regenerate when it changes
```

To create a new blog post do

```
rake new_post[new_meetup]
```

Edit the post using [Markdown](http://octopress.org/docs/blogging/) and then do

```
rake deploy
```

and this will commit the source and the master branches in one command.

If you don't have commit rights yet then fork the repo and send me a pull request on
the source branch and I will regenerate.

#### Why the high barrier to committing content.

If you are a coder / hacker then you know how to use git and can figure out how to use markdown. If
you pass this you probably are not a spammer




