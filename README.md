# Emerging Technology Atlas
https://emerging.digital.gov/



### Markdown
Needing a little help with Markdown? [Check out this handy cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).


### How to Link

Here is how to add a link in Markdown:

`[words you want to link](URL)`

Here is how to add a link to an internal page in Markdown:
1. find the filename that you'd like to link to, e.g. `pages/2018-2-14-Meeting.md`.
2. copy/paste that filename into this string: `{{ site.baseurl }}{% link pages/2018-2-14-Meeting.md %}`
3. use this as your "URL" in the regular markdown link format, e.g. <br>`[words you want to link]({{ site.baseurl }}{% link pages/2018-2-14-Meeting.md %})`


### How to Redirect

If you formerly had a page at: `https://emerging.digital.gov/vr/`

and have now moved it to
`https://emerging.digital.gov/virtual-reality/`

You'll need to add this bit of data to the front-matter to the new page that readers will read, in this case it is the `virtual-reality.md` file:

```
redirect_from:
  - /vrar/
```

If you have multiple paths, please add them like this:

```
redirect_from:
  - /vrar/
  - /space-goggles/
```
