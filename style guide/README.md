---
id: doc1
title: Style Guide
sidebar_label: Style Guide
---

You can write content using [GitHub-flavored Markdown syntax](https://github.github.com/gfm/).

## Markdown Syntax

To serve as an example page when styling markdown based Docusaurus sites.

## Headers

# H1 - No need to use this one (the article title is added automatically)

## H2 - Regular captation

### H3 - Create the best documentation

#### H4 - Create the best documentation

##### H5 - Create the best documentation

###### H6 - Create the best documentation

---

## Emphasis

Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~

### Superscript and subscript
<sup>....</sup>
<sub>....</sub>

Example:
Tidal volume is writting as V<sub>T</sub>

---

## Lists

1. First ordered list item
1. Another item
   - Unordered sub-list.
1. Actual numbers don't matter, just that it's a number
   1. Ordered sub-list
1. And another item.

* Unordered list can use asterisks

- Or minuses

+ Or pluses

---

## Images

All images need to be saved in the documents directory. The file name is constructed from the article id and counter like "2323423_1.png". 

It is added to the article using {{img|.....}}. Refer to the image number. Make sure to either use a citation counter from the end of the article ("ref=" followed by the reference number) or a direct hyperlink ("hyp="). The add your caption. 

{{img | img_nr=1 | doi=10.1007/s00134-020-06288-9}}
{{img | img_nr=1 | hyp=https://wikipedia.org|capt="Principles of lung and diaphragm-protective ventilation. ΔP: change in airway pressure during inspiration; PEEP: positive end-expiratory pressure; P-SILI: patient self-inflicted lung injury; VILI: ventilator-induced lung injury; VT: tidal volume"}}

---

## Code

```javascript
var s = 'JavaScript syntax highlighting';
alert(s);
```

```python
s = "Python syntax highlighting"
print(s)
```

```
No language indicated, so no syntax highlighting.
But let's throw in a <b>tag</b>.
```

```js {2}
function highlightMe() {
  console.log('This line can be highlighted!');
}
```

---

## Tables

Colons can be used to align columns.

| Tables        |      Are      |   Cool |
| ------------- | :-----------: | -----: |
| col 3 is      | right-aligned | \$1600 |
| col 2 is      |   centered    |   \$12 |
| zebra stripes |   are neat    |    \$1 |

There must be at least 3 dashes separating each header cell. The outer pipes (|) are optional, and you don't need to make the raw Markdown line up prettily. You can also use inline Markdown.

| Markdown | Less      | Pretty     |
| -------- | --------- | ---------- |
| _Still_  | `renders` | **nicely** |
| 1        | 2         | 3          |

---

## Blockquotes

> Blockquotes are very handy in email to emulate reply text. This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can _put_ **Markdown** into a blockquote.

---

## Inline HTML

<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

---

## Line Breaks

Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a _separate paragraph_.

This line is also a separate paragraph, but... This line is only separated by a single newline, so it's a separate line in the _same paragraph_.

---

## Admonitions

:::note

This is a note

:::

:::tip

This is a tip

:::

:::important

This is important

:::

:::caution

This is a caution

:::

:::warning

This is a warning

:::

## References, citation & hyperlinks

### References at the article's end
Use curly brackets and "cite journal" indicating a journal citation. Then use a counter and state the DOI. Use a "|" as a delimiter. Authors, title, journal, year of publication and hyperlink will be added automatically.  
{{cite journal | ref_nr=1 | doi=10.1093/bioinformatics/btn450}}

### Inline citation
Any citation anywhere in the text can be formulated as
{{cite inline | ref_nr=1}}
The number refers to the counter at the References section.
