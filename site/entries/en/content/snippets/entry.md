---
title: Snippets
---

<p>
    Snippets are extensions written on PHP/HTML/JS languages that add different features on the site.
</p>

<p>
    Snippets are stored in <code>/site/snippets/</code> <br>
    You can edit snippets manually using any text editor or via the admin panel in the snippets section.
</p>


<h3>Using snippets in the content</h3>

<p>
    You can display the snippet in the page with a shortcode like this:
</p>

<pre><code class="html hljs">&#91;snippet name="snippet_name"]</code></pre>

<h3>Snippets can be displayed in the template</h3>

<p>
    Display a snippet by its name:
</p>

<pre><code class="php hljs">&lt;?= Snippets::get('snippet_name') ?&gt;</code></pre>