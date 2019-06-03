# GitHub Flavored Markdown Workarounds

**Has GitHub not displayed your README.md or other Markdown the way you want it displayed?  Then please fork this repository, document your discrepancy and any workaround you have found, and submit a pull request.**

## Background
GitHub has its own [GitHub Flavored Markdown (GFM)](https://help.github.com/en/articles/about-writing-and-formatting-on-github) based on a [GitHub Flavored Markdown Spec](https://github.github.com/gfm).  The Spec guides GitHub's display of Markdown files, especially the ubiquitous README.md files found in nearly every repository hosted on GitHub.

Ironically, the Spec does not appear to have been written in GFM because it uses a feature not currently available in GFM: headings prefixed with a [decimal scheme](https://en.wikipedia.org/wiki/Outline_(list)#Decimal_outline). The Spec also does not appear to be available in a GitHub git repository so that we may fork it and suggest revisions through pull reqeusts.

When trying to understand Markdown, GFM, and [workarounds](https://en.wikipedia.org/wiki/Workaround), it can be helpful to remember that Markdown's "[key design goal is readability – that the language be readable as-is, without looking like it has been marked up with tags or formatting instructions, unlike text formatted with a markup language, such as Rich Text Format (RTF) or HTML, which have obvious tags and formatting instructions. To this end, its main inspiration is the existing conventions for marking up plain text in email](https://en.wikipedia.org/w/index.php?title=Markdown&oldid=899053982)".  Accordingly, workarounds that (a) produce the desired format for processed Markdown viewed on GitHub.com but (b) decrease the readability of the plain text Markdown file may be unsatisfactory.  However, it seems likely that most GitHub README.md files are _not_ read in plain text, at least not initially. So, let's see those workarounds!

## Workarounds

### Prefixed Headings, aka Numbered Headings

Outline headings with a decimal or alphanumeric [prefix scheme](https://en.wikipedia.org/wiki/Outline_(list)) are desirable.  The GFM Spec itself uses a decimal scheme.  However, GFM does not do numbered headings in plain Markdown.  You have to do a [workaround](PrefixedHeadingsInGFM.md) where you mix plain Markdown with HTML, and even then GitHub's style sheets can cause difficulties.

### _Your identified discrepancy and workaround here!_

_What does GFM not do for you, and what is your workaround, if any?_
