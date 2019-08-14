---
title: Media
---
<p>
    Entries can have any number and kind of images, videos, documents or other files.<br>
    Those files are being stored directly in the entry folder.
</p>
<h3>Getting list of images for entry in your template</h3>
<pre><code class="php hljs">&lt;?php $images = Filesystem::getFilesList(PATH['entries'] . '/portfolio', 'jpg') ?&gt;</code></pre>

<h3>Displaying images</h3>
<pre><code class="html hljs">&lt;?php foreach($images as $image): ?>
    &lt;img src="&lt;?= $entry['base_url'] . '/portfolio/' . basename($image); ?&gt;" /&gt;
&lt;?php endforeach ?&gt;
</code></pre>

<h3>Display images using the Glide/Intervention</h3>

<p>
    The built-in Glide/Intervention library allows you to do manipulations with images and cache the images.
</p>

<p>
    An example of using the Glide/Intervention library to resize images:
</p>

<pre><code class="html hljs">&lt;?php foreach($images as $image): ?>
    &lt;img src="&lt;?= Images::getImageUrl('portfolio/' . $image, ['w' => '670']) ?&gt;" /&gt;
&lt;?php endforeach ?&gt;
</code></pre>

<p>
    A complete list of available options, you can find here: <a href="http://glide.thephpleague.com/1.0/api/quick-reference/">http://glide.thephpleague.com/1.0/api/quick-reference/</a>
</p>