# AsciiDoc Article Title

This page is quoted from [the official Asciidoc Article Template](https://asciidoctor.org/docs/asciidoc-article/),
with a subsection "Include directive" added at the tail.

Firstname Lastname &lt;<author@asciidoctor.org>&gt;
3.0, July 29, 2022: AsciiDoc article template

Content entered directly below the header but before the first section heading is called the preamble.

## First level heading

This is a paragraph with a **bold** word and an *italicized* word.

![Image caption](image-file-name.png)

This is another paragraph.[1]

### Second level heading

-   list item 1

    -   nested list item

        -   nested nested list item 1

        -   nested nested list item 2

-   list item 2

This is a paragraph.

Content in an example block is subject to normal substitutions.

Sidebars contain aside text and are subject to normal substitutions.

#### Third level heading

**Listing block title**

    Content in a listing block is subject to verbatim substitutions.
    Listing block content is commonly used to preserve code input.

##### Fourth level heading

<table>
<caption>Table title</caption>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th style="text-align: left;">Column heading 1</th>
<th style="text-align: left;">Column heading 2</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;"><p>Column 1, row 1</p></td>
<td style="text-align: left;"><p>Column 2, row 1</p></td>
</tr>
<tr class="even">
<td style="text-align: left;"><p>Column 1, row 2</p></td>
<td style="text-align: left;"><p>Column 2, row 2</p></td>
</tr>
</tbody>
</table>

Table title

###### Fifth level heading

> I am a block quote or a prose excerpt.
> I am subject to normal substitutions.
>
> — 
> firstname lastname
> movie title

>     I am a verse block.
>       Indents and endlines are preserved in verse blocks.
>
> — 
> firstname lastname
> poem title and more

## First level heading

There are five admonition labels: Tip, Note, Important, Caution and Warning.

1.  ordered list item

    1.  nested ordered list item

2.  ordered list item

The text at the end of this sentence is cross referenced to [the third level heading](#_third_level_heading)

## First level heading

This is a link to the [Asciidoctor documentation](https://docs.asciidoctor.org/home/).
This is an attribute reference [that links this text to the AsciiDoc Syntax Quick Reference](https://docs.asciidoctor.org/asciidoc/latest/syntax-quick-reference/).

## Include directive

Here we include the source code of the file `src/main/java/my/Hello.java`.

    package my;

    public class Hello {
        public static void main(String[] args) {
            System.out.println("hello, world!");
        }
    }

[1] I am footnote text and will be displayed at the bottom of the article.
