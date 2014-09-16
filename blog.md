---
layout: archive
---
<div id="main" class="inner">
	<section class="clearfix">
		
		<div class="container-fluid">

			<div class="span12 top-title">
				<h2 class="post-title fadeInUp animated">Blog</h2>
		<ul>
			{% for post in site.posts %}
			<li class="pub-item">
			<span class="meta">{{ post.date | date_to_string }}</span>
			<a href="{{ post.url }}">
			<h3>{{ post.title }}</h3></a>
			{% if post.description %}
			<p>{{ post.description }}…<a href="{{ post.url }}">More</a></p>
			{% endif %}
			</li>
		</br>
			{% endfor %}
		</ul>
			</div>
		</div>
	</section>
</div>