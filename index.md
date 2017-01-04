---
layout: default
---

## Overview
The Toolbox Repository is a collection of [Atlas](http://www.ensoftcorp.com/atlas/) program analysis toolbox plugins. This site provides a simple composite update site to easily install a toolbox plugin and its dependencies.

## Installing Toolboxes
1. Start Eclipse, then select `Help` &gt; `Install New Software`.
2. Click `Add`, in the top-right corner.
3. In the `Add Repository` dialog that appears, enter &quot;Atlas Toolboxes&quot; for the `Name` and &quot;[https://ensoftcorp.github.io/toolbox-repository/toolboxes/](https://ensoftcorp.github.io/toolbox-repository/toolboxes/)&quot; for the `Location`.
4. In the `Available Software` dialog, select the checkbox next to each toolbox you wish to install and click `Next` followed by `OK`.
5. In the next window, you'll see a list of the tools to be downloaded. Click `Next`.
6. Read and accept the license agreements, then click `Finish`. If you get a security warning saying that the authenticity or validity of the software can't be established, click `OK`.
7. When the installation completes, restart Eclipse.

## Toolbox Overview
<div class="posts">
  {% for post in site.posts %}
    {% unless post.draft %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
   {% endunless %}
  {% endfor %}
</div>