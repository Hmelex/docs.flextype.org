---
title: Installation
---

<h2 class="margin-top-hard">Flextype Installation</h2>
<h3>Using (S)FTP</h3>
<p><a href="http://flextype.org/download">Download the latest version.</a>  </p>
<p>Unzip the contents to a new folder on your local computer, and upload to your webhost using the (S)FTP client of your choice. After you’ve done this, be sure to chmod the following directories (with containing files) to <code>755</code> (or <code>777</code>), so they are readable and writable by Flextype:  </p>
<ul>
<li><code>site/</code></li>
</ul>
<h3>Using Composer</h3>
<p>You can easily install Flextype with Composer.</p>
<pre><code>composer create-project flextype/flextype</code></pre>
<p>Also you may need to install vendor libs for Default Theme</p>
<pre><code>composer install
cd site/themes/default
npm install
gulp
</code></pre>
<h3>Using command-line</h3>
<p>If you have command-line access, you can easily install Flextype by executing a few commands. First, create the directory where you want to install Flextype, if it doesn’t already exist. Enter the directory, and execute the following commands:  </p>
<pre><code>wget https://github.com/flextype/flextype/releases/download/v0.8.3/flextype-0.8.3.zip
unzip flextype-0.8.3.zip
chmod -R 0777 site/</code></pre>

<h3>Installation issues</h3>
<h5>Broken subpages</h5>
<p>Your homepage is working, but subpages won't open or lead to a server error?</p>
<ol>
    <li>Make sure that the .htaccess file is present in your Flextype folder.</li>
    <li>Check if mod_rewrite is enabled on your server.</li>
    <li>Please try setting the RewriteBase in the .htaccess file:</li>
</ol>
<pre><code>RewriteBase /</code></pre>
<p>If you run Flextype in a subfolder, make sure to set the RewriteBase according to the name of your subfolder:</p>
<pre><code>RewriteBase /my-subfolder/</code></pre>

<br>

<h2>Themes Installation</h2>
<ol>
<li>Unzip theme to the folder <code>/site/themes/</code></li>
<li>Go to <code>/site/config/settings.yaml</code> and update <code>theme:</code> setting with your theme name.</li>
<li>Save your changes.</li>
</ol>
<p>Example:</p>
<pre><code>theme: theme-name</code></pre>

<br>

<h2>Plugins Installation</h2>
<ol>
<li>Unzip plugin to the folder <code>/site/plugins/</code></li>
</ol>