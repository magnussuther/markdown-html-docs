# Markdown-HTML Documentation

Easily present your Markdown documentation as a beatiful single-page HTML site. 


## Comparison with other common documentation tools

The graphic design is heavily influenced by Slate (https://github.com/lord/slate), but Markdown-HTML works in a different manner.

Whereas Slate is a static site generator (kind of like Jekyll that many are familiar with), Markdown-HTML is just a single HTML document linking to a script that downloads your Markdown files and renders it to HTML.
Markdown-HTML is simplier in that regard. 


### Cons
- Not ready for production yet. This is just a POC at this time.
- Probably not very performant.
- Makes a GET request for each of your Markdown files. You might want to consider using a static assets cache if you have a lot of files and high traffic loads.


### Pros
- Your gh-pages branch looks exactly like your master branch, so you can easily just merge a PR to get your docs online.
- No need to setup some tools to generate the documentation on your computer and then push it to the gh-pages branch.
- No dirt in your repository. You only need a very simple HTML document. See Usage below.
