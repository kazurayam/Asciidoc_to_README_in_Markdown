# Title

In a GitHub repository, you can make a file `README.adoc` in Asciidoc format.
GitHub happily renders the file in browser.
You can enjoy Asciidoc capabilities to author documents.

However, there is a defect.

GitHub-flavored-Asciidoc does not support `include::file/path/to/include[]` directive.

## Section

### Subsection

My first Java program is here:

    package my;

    public class Hello {
        public static void main(String[] args) {
            System.out.println("hello, world!");
        }
    }

### Subsection

A workaround developed by @chevdoor at 9th June 2021
at <https://github.com/github/markup/issues/1095>
You need to install `pandoc` and `asciidoctor`.
