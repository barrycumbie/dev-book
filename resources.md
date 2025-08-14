---
layout: default
title: Resources
permalink: /resources/
---

<div class="d-flex justify-content-between align-items-center mb-4">
    <h1><i class="fas fa-tools text-success me-3"></i>Development Resources</h1>
</div>

<div class="alert alert-success">
    <h5><i class="fas fa-lightbulb me-2"></i>Essential Tools & References</h5>
    <p class="mb-0">
        This collection includes essential tools, references, and best practices for web development. 
        Bookmark these resources for quick access during projects.
    </p>
</div>

<div class="row">
    {% assign resources = site.resources | sort: 'order' %}
    {% for resource in resources %}
    <div class="col-lg-6 mb-4">
        <div class="card h-100">
            <div class="card-body">
                <div class="d-flex justify-content-between align-items-start mb-3">
                    <h5 class="card-title mb-0">{{ resource.title }}</h5>
                    {% if resource.category %}
                    <span class="badge bg-success">{{ resource.category | replace: '-', ' ' | capitalize }}</span>
                    {% endif %}
                </div>
                
                {% if resource.subtitle %}
                <p class="card-text text-muted">{{ resource.subtitle }}</p>
                {% endif %}
                
                <p class="card-text">{{ resource.content | strip_html | truncatewords: 25 }}</p>
            </div>
            <div class="card-footer bg-transparent">
                <a href="{{ resource.url | relative_url }}" class="btn btn-success">
                    View Resource <i class="fas fa-external-link-alt ms-1"></i>
                </a>
            </div>
        </div>
    </div>
    {% endfor %}
</div>

<div class="row mt-5">
    <div class="col-lg-4">
        <div class="card">
            <div class="card-header">
                <h5 class="mb-0"><i class="fas fa-code me-2"></i>Development Tools</h5>
            </div>
            <div class="card-body">
                <ul class="list-unstyled">
                    <li><a href="{{ '/resources/vs-code-tips' | relative_url }}">VS Code Setup & Tips</a></li>
                    <li><a href="{{ '/resources/keyboard-shortcuts' | relative_url }}">Keyboard Shortcuts</a></li>
                    <li><a href="https://getbootstrap.com/" target="_blank">Bootstrap Documentation</a></li>
                    <li><a href="https://developer.mozilla.org/" target="_blank">MDN Web Docs</a></li>
                </ul>
            </div>
        </div>
    </div>
    
    <div class="col-lg-4">
        <div class="card">
            <div class="card-header">
                <h5 class="mb-0"><i class="fas fa-book me-2"></i>Learning Materials</h5>
            </div>
            <div class="card-body">
                <ul class="list-unstyled">
                    <li><a href="{{ '/resources/markdown-basics' | relative_url }}">Markdown Guide</a></li>
                    <li><a href="{{ '/resources/nato-phonetic' | relative_url }}">NATO Phonetic Reference</a></li>
                    <li><a href="https://www.codecademy.com/" target="_blank">Codecademy</a></li>
                    <li><a href="https://www.freecodecamp.org/" target="_blank">freeCodeCamp</a></li>
                </ul>
            </div>
        </div>
    </div>
    
    <div class="col-lg-4">
        <div class="card">
            <div class="card-header">
                <h5 class="mb-0"><i class="fas fa-heart me-2"></i>Health & Wellness</h5>
            </div>
            <div class="card-body">
                <ul class="list-unstyled">
                    <li><a href="{{ '/resources/ergonomics' | relative_url }}">Ergonomics & Well-Being</a></li>
                    <li><a href="https://justgetflux.com/" target="_blank">f.lux (Blue Light Filter)</a></li>
                    <li><a href="https://www.workrave.org/" target="_blank">Workrave (Break Reminder)</a></li>
                </ul>
            </div>
        </div>
    </div>
</div>

<div class="row mt-4">
    <div class="col-12">
        <div class="alert alert-info">
            <h5><i class="fas fa-question-circle me-2"></i>Need Help?</h5>
            <p class="mb-0">
                If you're looking for additional resources or have suggestions for this collection, 
                reach out via <a href="mailto:{{ site.email }}">email</a> or during office hours.
            </p>
        </div>
    </div>
</div>
