Markdown Smart Internal Links Extension for [Mecha](https://github.com/mecha-cms/mecha)
=======================================================================================

This extension will generate automatic link text and title attribute based on the page path provided. If the page file you are trying to provide does not exist, this extension will mark the automatic link with a red strikethrough text effect.

### Usage

The link syntax is exactly the same as referenced link syntax in **Markdown**, the only difference is that you need to add a `link:` prefix to the reference ID:

~~~ .markdown
[link:page-one] → will be replaced into `[Page Title](/directory/directory/page-one "Page Title")`
[link text][link:page-one] → will be replaced into `[link text](/directory/directory/page-one "Page Title")`
[link:does-not-exist] → will be replaced into `<s style="color:#f00;" title="[link:does-not-exist]">link broken</s>`
~~~

Release Notes
-------------

### 2.4.5

 - [@mecha-cms/mecha#96](https://github.com/mecha-cms/mecha/issues/96)
