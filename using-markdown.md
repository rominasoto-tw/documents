---
layout: page
title: Using Markdown
subtitle: A set of useful tips for beginners.
---

When I made the professional move from creating and editing PDF manuals to online documentation, the first challenge I encountered was the use of *Markdown*. While *Markdown* isn't difficult to use per se, at the end of the day I did need to know a bunch of ways to add or format certain content, so that the online output of my production looked the way I wanted it to.

In order to make this learning curve easier - and faster! - for me, I created a small *Markdown cheat sheet*. I kept it by my laptop and consulted it as needed. Before long, I found that I remembered what I had to do, and didnt need to consult my cheat sheet anymore.

This document offers you the same cheat sheet, so you can use it whiel you learn, just like I did. Good luck!

## Headings

Headings and their hierarchy are established using #

So, the way to create different sizes of titles and subtitles, like this:

![Titles example](/img/using-markdown/image-1.png)

Is to type them in this way, using #:

```
# Title 1
## Title 2
### Title 3
```

You can use this to create an information hierarchy in your documents, and to make the tables of contents of your online documentation easier to navigate.

&nbsp;

## Text Style

&nbsp;

### Bold Text

For **bold text** write this:

```
**example text**
```

&nbsp;

### Italic Text

For *italic text* write this:

```
*example text*
```

&nbsp;

### Bold & Italic Text

For ***bold & italic text*** write this:

```
***example text***
```

&nbsp;

### Underlined Text

For <ins>underlined text</ins> we can use GitHub markdown like this:

```
<ins>example text</ins>
```

&nbsp;

### Strikethrough Text

For ~~strikethroughs~~ write this:

```
~~example text~~
```

## Lists

You can create **ordered** and **unordered** lists in markdown.

&nbsp;

### Ordered Lists

For **ordered** lists like this:

1. First
2. Second
3. Third

Write this:

```
1. First
2. Second
3. Third
```

Note that if you write something like this with random numbers

```
1. First
27. Second
8. Third
```

Markdown will still make it look like this:

1. First
2. Second
3. Third

&nbsp;

### Unordered Lists

For **unordered** lists like this:

* First
* Second
* Third

Write this:

```
* First
* Second
* Third
```

or this:

```
- First
- Second
- Third
```

&nbsp;

## Code

To write `inline code` write this:

```
`example text`
```

To write a code block write this:

\```

this is an example

\```

The text will display "boxed", like this:

```
this is an example
```

You can also add syntax highlighting to the code:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

By writing this:

\```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
\```

You can also add line numbers to the code:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

By writing this:

```
{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}
```

&nbsp;

## Horizontal Rule

To add a horizontal rule like this:

---

You must write this:

```
---
```

&nbsp;

## Links

To add a link, use the following:

```
[link title](https://www.examplelink.com)
```

&nbsp;

## Images

To add an image, use the following:

```
![alt text](image.jpg)
```

&nbsp;

## Line Spacing

In markdown a regular empty line space is achieved by leaving an empty line in between paragraphs. So, this:

text

text

text

is written like this:

```
text

text

text
```

If you do this, leaving no empty lines in between:

```
text
text
text
```

This will be the result:

text text text

Also, Markdown will ignore double spacesbetween lines. So, if you write this:

```
text


text


text
```

You will still get a single empty line in between:

text


text


text

&nbsp;

## Tables

For a table like this:

| Title | Title |
| --- | --- |
| Text | Text |
| Text | Text | 

Use this format:

```
| Title | Title |
| --- | --- |
| Text | Text |
| Text | Text | 
```

&nbsp;

## Tasks List

For a tasks list like this:

- [x] Task 1
- [ ] Task 2
- [ ] Task 3 

User this format:

```
- [x] Task 1
- [ ] Task 2
- [ ] Task 3 
```

Consider that `[x]` will show the task as selected, while `[ ]` will show the task as unselected.

&nbsp;

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.

