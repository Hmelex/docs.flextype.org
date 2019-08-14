---
title: Entries
---

<p>Entries are the fundamental building-blocks of your site. Each entry in Flextype should contains <strong>entry header</strong> block in YAML format at the top of the file and <strong>entry content</strong> marked up using HTML + Shortcodes at the bottom of the file.</p>
<p>Here is a basic example (site/entries/my-entry/entry.html):</p>
<pre><code class="text hljs">---
title: My Entry
description: My entry description
---
My entry content.</code></pre>
<p>Between these triple-dashed lines, you can set predefined entry header variables or even create custom ones of your own. These variables will then be available to you to access in site templates.</p>
<h3>Entries and Urls structure in Flextype:</h3>
<table class="table"><thead><tr><th>Physical Location</th>
<th>URL</th>
</tr></thead><tbody><tr><td>site/entries/home/entry.html</td>
<td>/</td>
</tr><tr><td>site/entries/blog/my-post/entry.html</td>
<td>/blog/my-post</td>
</tr><tr><td>site/entries/a/very/long/url/entry.html</td>
<td>/a/very/long/url</td>
</tr></tbody></table>
<h3>Predefined Entries Header Variables</h3>
<p>Here is a list of predefined entry header variables with example values:</p>
<pre><code class="text hljs">title: Welcome title
description: Some welcome description here
keywords: key, words
visibility: draft (or or hidden or empty for published pages)
author:
&nbsp;&nbsp;name: Sergey Romanenko
&nbsp;&nbsp;email: awilum@msn.com
&nbsp;&nbsp;url: https://github.com/Awilum
date: 2019-01-01 08:00
robots: noindex, nofollow
template: default (allows you to use different templates in your theme)  </code></pre>
<h3>Custom Entry Header Variables</h3>
<p>You can create your own custom entry header variables using any valid YAML syntax.</p>
<p>Example:   </p>
<pre><code>author:
&nbsp;&nbsp;twitter: "@getflextype"</code></pre>