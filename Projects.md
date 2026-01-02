---
layout: page
title: Projects
permalink: /projects/
---

<div style="text-align: center; background-color: #f6f8fa; padding: 2rem; margin-bottom: 2rem; border-radius: 8px; border-left: 4px solid #0366d6;">
  <p style="font-size: 1.1rem; line-height: 1.8; color: #24292e; margin: 0; max-width: 800px; margin-left: auto; margin-right: auto;">
    Explore our portfolio of innovative projects that apply modern web development technologies to solve real-world problems. Each project demonstrates practical implementations of full-stack development, from system architecture to user experience, showcasing comprehensive skills in building production-ready applications.
  </p>
</div>

{% assign projects = site.projects | sort: "order" %}

{% assign project_colors = "FF9800,3B82F6,A7F3D0,8B5CF6,059669,FFFF00" | split: "," %}

<div style="display: grid; gap: 2rem; margin-top: 2rem;">
  {% for project in projects %}
    {% assign index = forloop.index0 %}
    {% assign color = project_colors[index] %}
    
    <div style="border-radius: 12px; overflow: hidden; box-shadow: 0 4px 12px rgba(0,0,0,0.1); transition: transform 0.2s, box-shadow 0.2s;">
      <a href="{{ project.url | relative_url }}" style="text-decoration: none; display: block;">
        <div style="padding: 2rem; background: linear-gradient(135deg, #{{ color }}20 0%, #{{ color }}40 100%); border-left: 6px solid #{{ color }};">
          <div style="margin-bottom: 1rem;">
            <h2 style="margin: 0; color: #24292e; font-size: 1.8rem;">{{ project.title }}</h2>
            {% if project.summary %}
              <p style="margin: 0.5rem 0 0 0; color: #586069; font-size: 1rem;">{{ project.summary }}</p>
            {% endif %}
          </div>
        </div>
        <!-- <div style="padding: 1.5rem 2rem; background-color: white; border-top: 1px solid #e1e4e8;">
          <span style="color: #0366d6; font-weight: 600; font-size: 0.95rem;">View Project Details →</span>
        </div> -->
      </a>
    </div>
  {% endfor %}
</div>

<style>
  div[style*="box-shadow"]:hover {
    transform: translateY(-4px);
    box-shadow: 0 6px 20px rgba(0,0,0,0.15) !important;
  }
</style>
