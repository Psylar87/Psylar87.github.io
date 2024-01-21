---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<div class="home">

  <h1 class="page-heading">Posts</h1>

  <ul class="post-list">
    {% assign archived_posts = site.posts | where: "archived", false %}
    {% for post in archived_posts %}
      <li>

<div class="post-meta">
	        <b class="post-author>">{{ post.author }},</b>


<b class="post-date>">{{ post.date | date: "%b %-d, %Y" }} </b>
          {% include read_time.html %}

</div>

<h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        <p>
		{{ post.content | strip_html | truncatewords:60 }}
		</p>
		<p>
			<a class="btn" href="{{ BASE_PATH }}{{ post.url }}">Read more...</a>
		</p>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>