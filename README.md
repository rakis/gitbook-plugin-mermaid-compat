>## Update for Gitbook >v3.0.0

>With the release of Gitbook 3+, a branch has been created to support the new style of plugin.  The plugin will function the same way, but will instead use the new Gitbook Plugin style.  You can check it out in the [github-3-upgrade branch](https://github.com/rakis/gitbook-plugin-mermaid-compat/tree/gitbook-3-upgrade), or install the plugin using the @beta flag in your gitbook plugin config.

# Mermaid plugin for Gitbook
[![npm version](https://badge.fury.io/js/gitbook-plugin-mermaid-compat.svg)](https://badge.fury.io/js/gitbook-plugin-mermaid-compat)

Plugin for [GitBook](https://github.com/GitbookIO/gitbook) which renders [Mermaid](https://github.com/knsv/mermaid) diagrams and flow charts detected in the book markdown.

## How to install it?

You can use install via **NPM**:

```
$ npm install gitbook-plugin-mermaid-compat
```


And use it for your book with in the book.json:

```
{
    "plugins": ["mermaid-compat"],
    "pluginsConfig": {
      "mermaid-compat": {
         "theme": "forest" // here to change the mermaid theme
      }
    }
}
```

## How to use it?

Just put the code into fenced code block and tag it **mermaid** key word like this:

    ```mermaid
    graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
    ```
