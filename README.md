# Include directive is not supported in Github-flavored Asciidoc --- a workaround

## Problem to solve

In a GitHub repository, you can make a file named `README.adoc` in [Asciidoc](https://asciidoc-py.github.io/index.html) format. GitHub is able to convert Asciidoc text to HTML runtime so that it renders in browsers. A sample is here:

-   [article.adoc](https://github.com/kazurayam/IncludeIsNotSupportedInGithubFlavoredAsciidoc-a_workaround/blob/master/article.adoc)

This looks very nice! You can enjoy the Asciidoc capabilities to author your documents and publish them in GitHub.
However, there is a caveat in GitHub Flavored Asciidoc. **GitHub Flavored Asciidoc does not support the `include::path/to/file[]` directive.** See the subsection titled "Include directive" at the tail of [article.adoc](https://github.com/kazurayam/IncludeIsNotSupportedInGithubFlavoredAsciidoc-a_workaround/blob/master/article.adoc).

![Include directive not working](docs/images/Include_directive_not_working.png)

I intended to embed the source code of my Java program into the article for reference. I expected to see something as follows.

Here we include the source code of the file `src/main/java/my/Hello.java`.

## Include directive

    package my;

    public class Hello {
        public static void main(String[] args) {
            System.out.println("hello, world!");
        }
    }

A workaround developed by @chevdoor at 9th June 2021
at <https://github.com/github/markup/issues/1095>
You need to install `pandoc` and `asciidoctor`.
