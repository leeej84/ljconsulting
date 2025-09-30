<!-- Blog page temporarily hidden - will be re-enabled when content is ready
---
layout: default
title: Blog
permalink: /blog/
---

<section class="section">
    <div class="container">
        <h1 class="section-title">Latest Insights</h1>
        <p class="section-subtitle">
            Stay updated with the latest trends in Microsoft technologies, Azure Cloud, and enterprise IT solutions.
        </p>
        
        <div class="card-grid">
            {% for post in site.posts limit:6 %}
            <div class="card">
                <div class="card-icon">
                    <i class="fas fa-blog"></i>
                </div>
                <h3 class="card-title">
                    <a href="{{ post.url | relative_url }}" style="color: var(--text-primary); text-decoration: none;">
                        {{ post.title }}
                    </a>
                </h3>
                <p class="card-description">
                    {{ post.excerpt | strip_html | truncate: 150 }}
                </p>
                <div style="margin-top: 1rem; color: var(--text-muted); font-size: 0.9rem;">
                    <i class="fas fa-calendar" style="margin-right: 0.5rem;"></i>
                    {{ post.date | date: "%B %d, %Y" }}
                    {% if post.author %}
                    <span style="margin-left: 1rem;">
                        <i class="fas fa-user" style="margin-right: 0.5rem;"></i>
                        {{ post.author }}
                    </span>
                    {% endif %}
                </div>
            </div>
            {% endfor %}
        </div>
        
        {% if site.posts.size > 6 %}
        <div style="text-align: center; margin-top: 3rem;">
            <a href="{{ '/blog/archive' | relative_url }}" class="btn btn-secondary">View All Posts</a>
        </div>
        {% endif %}
    </div>
</section>
-->
