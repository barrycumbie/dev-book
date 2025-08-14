---
layout: default
title: "Shared Lessons"
nav_order: 6
description: "Content lessons referenced by both CIS 376 and CIS 486"
---

# Shared Lessons
{: .fs-9 }

Content lessons that may be referenced by either course
{: .fs-6 .fw-300 }

These lessons are designed to be modular and reusable across both CIS 376 (Web Development) and CIS 486 (Capstone Projects). Each lesson focuses on specific skills or concepts that are valuable in multiple contexts.

---

## Available Lessons

{% assign lessons = site.lessons | sort: 'order' %}
{% if lessons.size > 0 %}
<div class="lesson-grid">
{% for lesson in lessons %}
  <div class="card mb-3">
    <div class="card-body">
      <h5 class="card-title">
        <a href="{{ lesson.url | relative_url }}">{{ lesson.title }}</a>
      </h5>
      {% if lesson.description %}
        <p class="card-text">{{ lesson.description }}</p>
      {% endif %}
      {% if lesson.courses %}
        <div class="course-tags">
          {% for course in lesson.courses %}
            <span class="badge bg-primary">{{ course }}</span>
          {% endfor %}
        </div>
      {% endif %}
      {% if lesson.topics %}
        <div class="topic-tags mt-2">
          {% for topic in lesson.topics %}
            <span class="badge bg-secondary">{{ topic }}</span>
          {% endfor %}
        </div>
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>
{% else %}
<div class="alert alert-info" role="alert">
  <h4 class="alert-heading">Lessons Coming Soon!</h4>
  <p>Shared lessons are currently being developed and will be available soon. These will include:</p>
  <ul>
    <li>Version Control with Git and GitHub</li>
    <li>Project Management Methodologies</li>
    <li>System Design Principles</li>
    <li>Testing and Quality Assurance</li>
    <li>Documentation Best Practices</li>
    <li>Presentation and Communication Skills</li>
  </ul>
</div>
{% endif %}

---

## Lesson Categories

### Development Skills
- Version control and collaboration
- Code organization and structure
- Testing and debugging
- Documentation practices

### Project Management
- Agile and Scrum methodologies
- Project planning and estimation
- Risk management
- Team collaboration

### Design and Architecture
- System design principles
- User experience considerations
- Database design
- API design and integration

### Professional Skills
- Technical communication
- Presentation skills
- Code review practices
- Industry best practices

---

## How to Use These Lessons

1. **For CIS 376 Students**: Focus on development and technical skills
2. **For CIS 486 Students**: Emphasize project management and architecture
3. **Cross-Reference**: Many concepts apply to both courses
4. **Self-Paced**: Work through lessons as needed for your projects

---

## Lesson Request

Have a topic you'd like to see covered? [Email Dr. Cumbie](mailto:{{ site.instructor.email }}) with your suggestions!
