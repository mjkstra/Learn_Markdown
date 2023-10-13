
# Learn Markdown  

# Table of contents

- [Titles and subtitles](#titles-and-subtitles)
- [Escapes](#escapes)
- [Paragraphs and formatting](#paragraphs-and-formatting)
- [Blockquotes](#blockquotes)
- [Lists](#lists)
  - [Unordered lists](#unordered-lists)
  - [Ordered lists](#ordered-lists)
- [Code](#code)
- [Horizontal Rule](#horizontal-rule)
- [Links](#links)
  - [External links](#external-links)
  - [Special links](#special-links)
  - [Compact links](#compact-links)
- [Images](#images)
- [Tables](#tables)
- [Footnotes](#footnotes)
- [Definition Lists](#definition-lists)
- [Task Lists](#task-lists)
- [Latex style math](#latex-style-math)
- [Emojis](#emojis)

<br>

## Titles and subtitles

To write titles you have to prepend up to **6 times** the **\#** character at the beginning of each line.  
The more **\#** you write, the smaller the title will be (subtitles).  
You should insert a line **before and after** the title in order to render it.  

Examples: `# Title` , `## Smaller title`  

That renders like:

# Title

## Smaller title

<br>

## Escapes

Some characters like:
- \`
- \*
- \_
- \-
- \[
- \]
- \(
- \)
- \<
- \>

Are reserved and hence you should escape them with **\\**

<br>

## Paragraphs and formatting

This is a paragraph.  
To write a new line you should write **2 spaces** and press **enter** or you can use the **`<br>`** tag.

You can format the text in various ways:

- Italic: `t*ex*t, *text* or _text_`, that renders like: t*ex*t, *text* or _text_  
- Bold: `**text** or __text__ bold`, that renders like: **text** or __text__ bold  
- Bold and italic: `***text***, ___text___  or t***ex***t`, that renders like: ***text***, ___text___  or t***ex***t  
- Strikethrough: `~text~`, that renders like: ~text~  
- Monospaced: `` `text` ``, that renders like: `text`  

> **Note**: It is possible to remove the blue underlining from links by using the monospace formatting.  
> Eg: https://www.wikipedia.org can be turned into `https://www.wikipedia.org` to remove the blue underline.

<br>

## Blockquotes

To write a block quote write on each line a **\>** symbol.  
Blockquotes can be nested by adding multiple **\>** symbols.  
It is good practice to add a line before the beginning and after the end of the blockquote.  

Example:  

```
> This is a blockquote.   
> > They can also be indented like this.
```

Rendering:  

> This is a blockquote.   
> > They can also be indented like this.

<br>

## Lists

### Unordered lists

To write unordered lists you just need to write the **\-** character and a new line for each line.  
Lines can be indented with a **tab** or **4 spaces**.  

Example:  

```
- First unordered line
  - Second unordered line with indentation
```  

That renders like:  

- First unordered line  
  - Second unordered line with indentation

### Ordered lists

To write ordered lists, you just need to write a number followed by a \. and a new line at the end.  
Example:  
```
1. Ordered line  
```  

That renders like:  

1. Ordered Line  

***

If you would like to place and indent an unordered list, you need to write **4 spaces** before each line of the list.  

Example:  

```
2. Ordered line  
    - Unordered list with indentation  
```  

That renders like:  

2. Ordered line  
    - Unordered line with indentation  

***

If you would like to add code below a list entry you can write **8 spaces** for each line of code and **leave an empty line at the beginning** ( there is also a much more elegant way, with sintax highlighting explained in the next chapter ).  

Example:  

```
3. Ordered line entry with code below  
        <html>
          <head>
            <title>titolo</title>
          </head>
        </html>
```  

That renders like:  

3. Ordered line entry with code below  
        <html>
          <head>
            <title>titolo</title>
          </head>
        </html>

***

If you would like to add comments, you need to write a new line, followed by **4 spaces** and then your comment.  

Example:  

```
4. Ordered line with comment below  
    A comment.
```  

That renders like:  

4. Ordered line with comment below  
    A comment.

***

You can also add an image below line entries by prepending **4 spaces** as prelude( images are explained later ).  

Example:  

```
5. Ordered line with image below:  
    ![Delicious Apple](./images/apple.png)
```  

That renders like:  

5. Ordered line with image below:  
    ![Delicious Apple](./images/apple.png)

<br>

## Code

By encapsulating text blocks around **double backticks \`\`** , you can write special characters without escaping them, like so:

`` For example I can write single backticks here ` without the need to escape them ``  

To write a block of code you need to prepend **4 spaces** to each line, like so:  

    <html>
        <head>
            <title>titolo</title>
        </head>
    </html>

<br>

Or else you can write code blocks inside a block delimited by **triple backticks \`\`\`** , with the possibility to exploit sintax highlighting, by stating the language used after the 3 opening backticks( I am sorry, but there's no way to show an example here because of MarkDown I can only show you the result. Check the raw format of this file to see how it's done ):  

```C++
//Some C++ code
int var = 2;
```

<br>

## Horizontal Rule

You can write an horizontal rule in multiple ways, just remember to add a line before and after.  
Here are some examples:

- 1st method: with **\*\*\***

***

- 2nd method: with **\_\_\_**

___

- 3rd method: with **\-\-\-**

---

<br>

## Links

### External links

You can write a link, like so: `[Wikipedia](https://www.wikipedia.org)`, with this effect: [Wikipedia](https://www.wikipedia.org)  
You can also add a tooltip, like so: `[Wikipedia](https://www.wikipedia.org "A site to share and learn information")`  , with this effect: [Wikipedia](https://www.wikipedia.org "A site to share and learn information")  

> **Note** : Tooltips can also be added with **\( \)**  

The link text can be formatted:  

- Bold links: [**Wikipedia**](https://www.wikipedia.org)  
- Italic links: [*Wikipedia*](https://www.wikipedia.org)  
- Monospace links: [`Wikipedia`](https://www.wikipedia.org)

<br>

### Special links

- Local link: `[Links](#links)` that renders -> [Links](#links)  
- Extended link: `<https://www.wikipedia.org>` that renders -> <https://www.wikipedia.org>  
- Mail link: `<mymail@gmail.com>` that renders -> <mymail@gmail.com>  

<br>

### Compact links

You can write compact links with this sintax: `[Wikipedia][1]`

Then define `[1]`, like so: `[1]: https://www.wikipedia.org "tooltip"`  

Try it here: [Wikipedia][1]

[1]: https://www.wikipedia.org "commento"

<br>

> **Note**: For compatibility reasons, if there are spaces in the link write **%20%** instead of them.

<br>

## Images  

There are several ways to add images: 

1. Standard: `[![Delicious Apple](./images/apple.png)]`  
2. With a tooltip: `![Delicious Apple](./images/apple.png "A red apple")`  
3. With an embedded link:  `[![Delicious Apple](./images/apple.png)](https://www.wikipedia.org/wiki/Apple)`  

Here is an example of an image with a tooltip and an embedded link:  
[![Delicious Apple](./images/apple.png "A red apple")](https://www.wikipedia.org/wiki/Apple)

<br>

## Tables
 
You can write tables like so:  

```
| Name | Surname | 
| --- | --- |
| Michele | G. |
```

That renders like this:  

| Name | Surname | 
| --- | --- |
| Michele | G. |

You can also set an alignment for each column and choose different text formatting for every cell, like so:  

```
| nome | cognome | nascita |
| :--- | :---: | ---: |
| *M.* | **G.** | `2001` |
```  

That renders like this:  

| nome | cognome | nascita |
| :--- | :---: | ---: |
| *M.* | **G.** | `2001` |

<br>

## Footnotes

> **Disclaimer:** They are not available in every markdown renderer.  

You can add footnotes in the text by using this sintax: `[^1]` or `[^sampletext]`.  

Example: `Hi, my name is Michele[^1] and I am a C programmer[^sampletext].`  

Then describe the footnotes:  

```
[^1]: First footnote.
[^sampletext]: Second footnote.
```

Everything will be rendered like this:  

Hi, my name is Michele[^1] and I am a C programmer[^sampletext]  

[^1]: First footnote.  
[^sampletext]: Second footnote.

<br>

## Definition Lists

> **Disclaimer:** They are not available in every markdown renderer.  
  
You can create definitions like so:  

```
Word1
: Definition1

Word2
: Definition1
: Definition2
```  

They will be rendered like this ( Github won't render them, I am sorry ):  

Word1
: Definition1

Word2
: Definition1
: Definition2

<br>

## Task Lists

> **Disclaimer:** They are not available in every markdown renderer.  

They consist of lists of checkboxes, usage:  

```
- [x] Done task
- [ ] Task to do
```

It will be rendered like this:  
- [x] Done task
- [ ] Task to do

<br>

## Latex style math  

> **Disclaimer:** They are not available in every markdown renderer. On Github it works thanks to Katex.  

To enter math mode there are two ways:  
- Writing in-line formulas by delimiting the text with \$ and \$ and without spaces between the dollar signs and the beginning and ending of the formula.  
- Writing block formulas by delimiting the text with \$\$ and \$\$ and without spaces between the dollar signs and the beginning and ending of the formula.  

An example of a block formula: `$$\int\limits_a^b{f(x)}$$ `  

That renders like this:  
$$\int\limits_a^b{f(x)}$$  

## Emojis

> **Disclaimer:** They are not available in every markdown renderer.  

You can insert emojis by coping them from an online database such as [EmojiPedia][2] or insert shortcodes like `:joy:` , that renders like :joy:.  
You can find [here][3] an online database with a lot of shortcodes, but the site seems down, rn.  

[2]: https://emojipedia.org/ "Emoji Database"
[3]: https://gist.github.com/rxaviers/7360908
