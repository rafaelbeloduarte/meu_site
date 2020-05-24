+++ 
draft = true
date = 2020-01-04T17:10:06-03:00
title = "Instructions for the usage of Markdown"
description = "Markdown é uma linguagem de marcação utilizadas nas publicações deste site."
slug = "markdown" 
tags = ['markdown', 'programação']
categories = []
externalLink = ""
series = []
toc = true
+++

Source: Adam Pritchard, [https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

License: [CC-BY](https://creativecommons.org/licenses/by/3.0/)

Modified by: Rafael

Markdown is the markup language used to write the posts on this website. I leave this cheat sheet here to facilitate my work when writing articles. It was originally written by Adam Pritchard, but it is not endorsed by him, I modified it and published here just to help write my posts, as permitted by [CC-BY](https://creativecommons.org/licenses/by/3.0/).

## Table of contents

To include table of contents conditionally, edit the file `single.html` in the directory `/themes/hugo-coder/layouts/posts`:

1. Locate the line:

```
{{ partial "post_meta.html" . }}
```

2. Below it, add the following:

```
{{ if .Params.toc }}
{{ .TableOfContents }}
{{ end }}
```

3. To enable Table of Contents set `toc = true` on the header. Example:

```
+++ 
draft = false
date = 2020-01-04T17:10:06-03:00
title = "Instructions for the usage of Markdown"
description = "Markdown é uma linguagem de marcação utilizadas nas publicações deste site."
slug = "instruções-para-utilização-de-markdown" 
tags = ['markdown', 'programação']
categories = []
externalLink = ""
series = []
toc = true
+++
```

Source: [https://www.codeooze.com/webdesign/hugo-toc/](https://www.codeooze.com/webdesign/hugo-toc/)

## Headers

```md
# H1
## H2
### H3
#### H4
##### H5
###### H6

Alternatively, for H1 and H2, an underline-ish style:

Alt-H1
======

Alt-H2
------
```

[Topo](#top)

## Emphasis

```
Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~
```

Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~

[Topo](#top)

## Lists

(In this example, leading and trailing spaces are shown with with dots: ⋅)

```
1. First ordered list item
2. Another item
⋅⋅* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
⋅⋅1. Ordered sub-list
4. And another item.

⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this line is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses
```
1. First ordered list item
2. Another item
⋅⋅* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
⋅⋅1. Ordered sub-list
4. And another item.

	You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

	To have a line break without a paragraph, you will need to use two trailing spaces.
	Note that this line is separate, but within the same paragraph.
	(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses

[Topo](#top)

## Links

There are two ways to create links.

```
[I'm an inline-style link](https://www.google.com)

[I'm an inline-style link with title](https://www.google.com "Google's Homepage")

[I'm a reference-style link][Arbitrary case-insensitive reference text]

[I'm a relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com> and sometimes 
example.com (but not on Github, for example).

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com
```

[I'm an inline-style link](https://rafaelbeloduarte.github.io)

[I'm an inline-style link with title](https://rafaelbeloduarte.github.io "Homepage")

[I'm a reference-style link][Arbitrary case-insensitive reference text]

[I'm a relative reference to a repository file](../)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com> and sometimes 
example.com (but not on Github, for example).

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

To open links in new tabs, do as recommended by [PrasadPen](https://discourse.gohugo.io/t/how-to-open-link-in-new-tab-with-hugos-new-goldmark-markdown-renderer-in-v0-62-0/22540):
> If you just want to be able to open links in new tab for your Hugo site, create a file (in the theme folder) at `layouts/_default/_markup/render-link.html` with the following content:

```
<a href="{{ .Destination | safeURL }}"{{ with .Title}} title="{{ . }}"{{ end }}{{ if strings.HasPrefix .Destination "http" }} target="_blank"{{ end }}>{{ .Text }}</a>
```
[Topo](#top)

## Images

```
Here's our logo (hover to see the title text):

Inline-style: 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Reference-style: 
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"
```

Here's our logo (hover to see the title text):

Inline-style: 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Reference-style: 
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"

[Topo](#top)

## Code and Syntax Highlighting

Code blocks are part of the Markdown spec, but syntax highlighting isn't. However, many renderers -- like Github's and Markdown Here -- support syntax highlighting. Which languages are supported and how those language names should be written will vary from renderer to renderer. Markdown Here supports highlighting for dozens of languages (and not-really-languages, like diffs and HTTP headers); to see the complete list, and how to write the language names, see the highlight.js demo page.

```
Inline `code` has `back-ticks around` it.
```

Inline `code` has `back-ticks around` it.

Blocks of code are either fenced by lines with three back-ticks ` ``` `, or are indented with four spaces. I recommend only using the fenced code blocks -- they're easier and only they support syntax highlighting.

```
	```javascript
	var s = "JavaScript syntax highlighting";
	alert(s);
	```

	```python
	s = "Python syntax highlighting"
	print s
	```

	```
	No language indicated, so no syntax highlighting. 
	But let's throw in a <b>tag</b>.
	```
```

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

```python
s = "Python syntax highlighting"
print s
```

```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```
[Topo](#top)

## Tables

Tables aren't part of the core Markdown spec, but they are part of GFM and Markdown Here supports them. They are an easy way of adding tables to your email -- a task that would otherwise require copy-pasting from another application.

```
Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
```

Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

[Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)

[Topo](#top)

## Math

To display math equations this page uses [MathJax](https://www.mathjax.org/), a JavaScript display engine for mathematics.

Usage:

Math expressions must be typed between `$`.

```tex
$
e^{i\pi} = -1
$
```
$
e^{i\pi} = -1
$

For centralized text use two dolar signs `$$`.

```tex
$$
e^{i\pi} + 1 = 0
$$
```
$$
e^{i\pi} + 1 = 0
$$

For special characters use backslashes and the name of the character. Examples:

```tex
$$
\pi \lambda \gamma \theta \alpha \beta \sigma \mu \kappa \zeta \psi \tau \rho \nu \eta \epsilon \delta \phi \omega
$$
```
$$
\pi \lambda \gamma \theta \alpha \beta \sigma \mu \kappa \zeta \psi \tau \rho \nu \eta \epsilon \delta \phi \omega
$$

To write uppercase letters make the fisrt one uppercase.

> On the Greek alphabet some uppercase letters are the same as in the Latin alphabet, for those just use your keyboard, their names won't work.

```tex
$$
\Pi \Lambda \Gamma \Theta A B \Sigma M K Z \Psi T P N H E \Delta \Phi \Omega
$$
```

$$
\Pi \Lambda \Gamma \Theta A B \Sigma M K Z \Psi T P N H E \Delta \Phi \Omega
$$

You can check the Greek alphabet [here](https://www.rapidtables.com/math/symbols/greek_alphabet.html).

To number equations I use `\label{eqi} \tag{i}` right after the equation.

```tex
$$
e^{i\pi} + 1 = 0
\label{eq1} \tag{1}
$$
```

$$
e^{i\pi} + 1 = 0
\label{eq1} \tag{1}
$$

You can then reference the equation using:
```
\ref{eq1}
```

Like this: Equation \ref{eq1} is Euler's identity.

For fractions we have `\frac`.

```tex
$$
\frac{df}{dt} = \displaystyle \lim_{h \to 0} \frac{f(t+h) - f(t)}{h}
$$
```

$$
\frac{df}{dt} = \displaystyle \lim_{h \to 0} \frac{f(t+h) - f(t)}{h}
$$

For more, here are some great guides: [Writing Mathematic Formulas in Markdown](http://csrgxtu.github.io/2015/03/20/Writing-Mathematic-Fomulars-in-Markdown/) by Archer Reilly and [Mathematics in R Markdown](https://www.calvin.edu/~rpruim/courses/s341/S17/from-class/MathinRmd.html) by R Pruim.

[Topo](#top)

## Citations

References or citations are shown at the botton of the page. They are done in the following manner.

```
Lorem ipsum dolor sit amet[^fn], consectetur adipiscing elit[^fn1].

[^fn]: Reference 1.

[^fn1]: Reference 2.
```

Lorem ipsum dolor sit amet[^fn], consectetur adipiscing elit[^fn1].

[^fn]: Reference 1.

[^fn1]: Reference 2.

## Blockquotes

```
> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote. 
```

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote. 

[Topo](#top)

## Inline HTML

You can also use raw HTML in your Markdown, and it'll mostly work pretty well.

```
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>
```

Not this time :(

<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

[Topo](#top)

## Horizontal Rule

```
Three or more...

---

Hyphens

***

Asterisks

___

Underscores
```

Three or more...

---

Hyphens

***

Asterisks

___

Underscores

[Topo](#top)

## Line Breaks

My basic recommendation for learning how line breaks work is to experiment and discover -- hit `<Enter>` once (i.e., insert one newline), then hit it twice (i.e., insert two newlines), see what happens. You'll soon learn to get what you want. "Markdown Toggle" is your friend.

Here are some things to try out:

```
Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a *separate paragraph*.

This line is also a separate paragraph, but...
This line is only separated by a single newline, so it's a separate line in the *same paragraph*.
```

Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a *separate paragraph*.

This line is also a separate paragraph, but...
This line is only separated by a single newline, so it's a separate line in the *same paragraph*.

(Technical note: Markdown Here uses GFM line breaks, so there's no need to use MD's two-space line breaks.)

[Topo](#top)

## YouTube Videos

They can't be added directly but you can add an image with a link to the video like this:

```
<a href="http://www.youtube.com/watch?feature=player_embedded&v=YOUTUBE_VIDEO_ID_HERE
" target="_blank"><img src="http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>
```

Or, in pure Markdown, but losing the image sizing and border:

```
[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](http://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)
```

Referencing a bug by #bugID in your git commit links it to the slip. For example #1.

[Topo](#top)

---

License: [CC-BY](https://creativecommons.org/licenses/by/3.0/)
