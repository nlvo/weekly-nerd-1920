---
layout: default
---

<h2>🗒 Notes</h2>
<section class="post-list">
	{% for post in site.notes %}
	<article>
		<h3>
			<a class="post-link" href="{{ post.url }}" title="{{ post.title }}">
				{{ post.title }}
			</a>
		</h3>
	</article>
	{% endfor %}
</section>

<h2>🚨 Articles</h2>
<section class="post-list">
	{% for post in site.articles %}
	<article>
		<!-- <time class="post-meta" datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time> -->
		<h3>
			<a class="post-link" href="{{ post.url }}" title="{{ post.title }}">
				{{ post.title }}
			</a>
		</h3>
	</article>
	{% endfor %}
</section>