---
title: Configuration
---
<p>Flextype allows you to configure your site in any way you can dream up, and it’s thanks to the powerful and flexible configuration options that make this possible. Configuration files are written in YAML syntax with a .yaml file extension. YAML is a data serialisation language designed to be directly writable and readable by humans. You can check out this <a href="https://learnxinyminutes.com/docs/yaml/">YAML help page</a> to get a complete understanding of the syntax available.</p>

<p>You can update and create site configuration by editing file <code>/site/config/settings.yaml</code></p>

<pre><code class="yaml"># The title of the website
title: "Site title here"

# The description of the website
description: "Site description here"

# The name and email address of the website author
author:
  email: ""
  name: ""

# Set the timezone to be used on the website.
# For a list of valid timezone settings, see:
# http://php.net/manual/en/timezones.php
timezone: UTC

# Charset
#
# Set internal character encoding.
#
# Currently the following names are supported:
# http://php.net/manual/ru/function.mb-regex-encoding.php#121645
charset: UTF-8

# Valid date format
# see: http://php.net/manual/ru/function.date.php
date_format: "F d Y H:i:s."

# The theme to use.
#
# Don't edit the provided theme templates directly, because they get updated
# in next releases. If you wish to modify a default theme, copy its folder, and
# change the name here accordingly.
theme: simple

# The locale that'll be used by the Flextype.
locale: "en"

# The default page to use for the homepage.
entries:
  main: home
  error404:
    title: 'Error 404'
    description: 'We''re sorry but the page you are looking for doesn''t appear to exist!'
    content: 'We''re sorry but the page you are looking for doesn''t appear to exist!'
    template: default

# Display errors
errors:
  display: true

# Cache
# available drivers: auto (will get one from installed cache drivers), apcu,
# apc, wincache, xcache, memcache, memcached, redis, file.
cache:
  enabled: true
  prefix: Flextype
  driver: auto
  lifetime: 604800

# Define the file types (extensions to be exact) that are acceptable for upload.
accept_file_types: [ gif, jpg, jpeg, png, ico, zip, tgz, txt, md, doc, docx, pdf, epub, xls, xlsx, ppt, pptx, mp3, ogg, wav, m4a, mp4, m4v, ogv, wmv, avi, webm, svg]
</code></pre>

Also you can update site setting in Admin Panel on the Settings page.