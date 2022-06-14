# GitHub Markdown Cheatsheet

Markdown is a lightweight markup language, mostly used for writing readmes. Each platform supporting Markdown usually adds its own flavors to it. GitHub is no exception, just recently adding support for writing mathematical formulae.

## TL;DR
**Thi**s **i**s a **GitH**ub-**flavor**ed **Markdo**wn **cheatshe**et **focusi**ng **o**n **les**s-**kno**wn **featur**es.[^1]

## Headings
Similar to HTML, there are 6 headings in Markdown:

```markdown
# H1
## H2
### H3
#### H4
##### H5
###### H6
```

Try to use heading level 1 for the title of your document, h2 for the sections, h3 for subsections, and so on.

## Alternate Headings
There is an alternate way of creating headings that only supports two levels:

```markdown
Heading Level 1
===============

Heading Level 2
---------------
```

## Paragraphs
Paragraphs are chunks of text separated by at least a blank line:

```markdown
This is paragraph 1.

This is paragraph 2.
```

## Line Breaks
Line break is less know to the Markdown world.  
It is achieved by adding at least two spaces to the end of the line:

```markdown
This is line 1.  
This is line 2.
```

It's less known, because it's invisible. But, try it out.

## Emphasis

There are three ways to emphasize:
- Bold
- Italic
- Bold and italic

Making bold can be done by double underscores or double asterisks:

```markdown
This is __bold__, so is **this**.
```

But inside a word, only the asterisks work:

```markdown
**Thi**s **i**s a **GitH**ub-**flavor**ed **Markdo**wn **cheatshe**et **focusi**ng **o**n **les**s-**kno**wn **featur**es.
```

To make italic, use one underscore or one asterisk, and again, inside a middle only the asterisk syntax works:

```markdown
This is _italic_, so is *this*. And it's not *un*important.
```

And to make something bold and italic, one can mix the two syntaxes:

```markdown
All of these are: ***bandi***, _**bandi**_, **_bandi_**, __*bandi*__, *__bandi__*, ___bandi___.
And inside the word: b***and***i which means bold***and***italic.
```

## Inline Code

To write code in monospace font inside a regular text, enclose it in backticks:

```markdown
This is `code` inside text.
```

If you want to write a code that has backticks in it, you can use double-backticks:

```markdown
This is the syntax: ``This is `code` inside a text.``
```

## Code Block

To create a code block, put four lines or a tab before it:

```markdown
This is the code:

    for i in range(10):
        pass
```

The alternative syntax is wrapping the code in three backticks.

````markdown
This is the code:

```
for i in range(10):
    pass
```
````

To display triple backticks in a code block, wrap them inside quadruple backticks.

````markdown
The alternative syntax is wrapping the code in three backticks.

``‌``
This is the code:

```
for i in range(10):
    pass
```
``‌``
````

To display triple and quadruple backticks inside a code block, wrap them inside quadruple backticks and put a [zero-width non-joiner](https://unicode-explorer.com/c/200C) inside the quadruple backticks you want to display.

## Code Block with Syntax Highlighting

To create a code block with syntax highlighting, you can use the three backtick syntax and write the language name in front of it:

```markdown
This is the code:

`‌`‌`python
for i in range(10):
    pass
`‌`‌`
```

As of now, some 583 languages are being supported for syntax highlighting. You can access the full list [here](https://github.com/github/linguist/blob/master/vendor/README.md).

## Blockquotes

Blockquotes are designated by a `>` in front of them:

```markdown
> Veniet tempus quo ista quae nunc latent in lucem dies extrahat et longioris aevi diligentia.
```

Use double `>` to create nested blockquotes.

> Georg Cantor quoted:
>
>> Veniet tempus quo ista quae nunc latent in lucem dies extrahat et longioris aevi diligentia.

## Ordered Lists

To create an ordered list:

```markdown
1. First item
2. Second item
3. Third item
```

The number can be out of order:
```markdown
1. First item (indexed 1)
1. Second item (indexed 1)
5. Third item (indexed 5)
```

Markdown still fixes the counters and outputs the correct numbers:

1. First item (indexed 1)
1. Second item (indexed 1)
5. Third item (indexed 5)

## Unordered Lists

To create unordered lists, use any of the following "bullet characters": hyphen `-`, asterisk `*`, or plus sign `+`:

```markdown
- Item
- Another item
- Yet another item
```

One can mix the bullet characters in one list, but it's a bad practice.

## Task Lists

A task list (aka _checklist_ or _todo list_) is an unordered list with each item having a checkbox in front, either checked or unchecked. Tasks lists are very useful when writing issues on GitHub, as one can then check or uncheck them without manually editing the Markdown source of the comment or description.

```markdown
- [x] Write the tests
- [ ] Implement the functions
- [ ] Fix the code formatting
```

Output:

- [x] Write the tests
- [ ] Implement the functions
- [ ] Fix the code formatting


## Horizontal Line

To create a horizontal line, use three or more asterisks (`***`), hyphens (`---`), or underscores (`___`):

```markdown
Some text!

---

Next chapter or something!
```

## URLs and Email Addresses

To turn URLs and email addresses into links, just wrap them into angle brackets:

```markdown
Take a look at my Medium posts: <https://aerabi.medium.com>
You can also email me at <mohammad-ali@aerabi.com>
```

## Links

To create a link, enclode the linked text in brackets and then immediately the URL in parentheses:

```markdown
Take a look at my [Medium posts](https://aerabi.medium.com/).
```

You can also add a title to the link that shows as a tooltip:

```markdown
Take a look at my [Medium posts](https://aerabi.medium.com/ "Git Weekly is published there!").
```

Take a look at my [Medium posts](https://aerabi.medium.com/ "Git Weekly is published there!").

## Images

Image syntax is similar to that of links, only it has an exclamation mark in front and the text is the alt text:

```markdown
![My GitHub avatar](https://avatars.githubusercontent.com/u/44623032?v=4)
```

[^1]: Here I made the words half bold. It showcases two things: 1. Making texts bold in the middle of the word. 2. Markdown footnotes. It is known that making the words half bold makes it easier and faster for your mind to read it. It's called bionic reading.
