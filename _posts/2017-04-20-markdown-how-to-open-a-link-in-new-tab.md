---
layout: post
title: Open markdown link in new tab
tags: Web Technology Jekyll
categories: [ blog, technology]
---

Linking in markdown is a fairly simple. You add the text in square brackets and enclose the link in parenthesis.

```markdown
[text-to-highlight](actual-link)
```

Now, to add a target attribute to the link

```markdown
[text-to-highlight](actual-link){:target="_blank"}
```
### Example

[Google](https://www.google.com/){:target="_blank"}

```markdown
[Google](https://www.google.com/){:target="_blank"}
```
