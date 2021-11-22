# Adding a NEWS item

Adding a news item is simple. Use the front matter below, add any content as HTML. Individual news items can be shown setting the `visible` flag true. The visible news items are sorted decending by date, i.e., the newest is at the top.


```
---
layout: plain
date: YYYY-MM-DD
visible: true/false
---

<h3>Title</h3>
<span class="font-small">Month DD, YYYY</span>
<p>
    Content
</p>

```