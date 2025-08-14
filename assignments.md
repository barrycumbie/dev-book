---
layout: default
title: Assignments
permalink: /assignments/
---

<div class="d-flex justify-content-between align-items-center mb-4">
    <h1><i class="fas fa-tasks text-primary me-3"></i>Course Assignments</h1>
</div>

<div class="alert alert-info">
    <h5><i class="fas fa-info-circle me-2"></i>Assignment Overview</h5>
    <p class="mb-0">
        This course includes three major projects (Alpha, Bravo, Charlie) plus smaller assignments. 
        Each project builds on previous skills while introducing new concepts.
    </p>
</div>

<div class="row">
    {% assign assignments = site.assignments | sort: 'order' %}
    {% for assignment in assignments %}
    <div class="col-lg-6 mb-4">
        <div class="card h-100">
            <div class="card-body">
                <div class="d-flex justify-content-between align-items-start mb-3">
                    <h5 class="card-title mb-0">{{ assignment.title }}</h5>
                    {% if assignment.points %}
                    <span class="badge bg-primary">{{ assignment.points }} pts</span>
                    {% endif %}
                </div>
                
                {% if assignment.subtitle %}
                <p class="card-text text-muted">{{ assignment.subtitle }}</p>
                {% endif %}
                
                <div class="mb-3">
                    {% if assignment.due_date %}
                    <small class="text-muted">
                        <i class="fas fa-calendar me-1"></i>Due: {{ assignment.due_date }}
                    </small>
                    {% endif %}
                    {% if assignment.difficulty %}
                    <div class="mt-1">
                        <small class="text-muted me-2">Difficulty:</small>
                        {% for i in (1..5) %}
                            {% if i <= assignment.difficulty %}
                                <i class="fas fa-star text-warning"></i>
                            {% else %}
                                <i class="far fa-star text-muted"></i>
                            {% endif %}
                        {% endfor %}
                    </div>
                    {% endif %}
                </div>
                
                {% if assignment.technologies %}
                <div class="mb-3">
                    {% for tech in assignment.technologies %}
                    <span class="badge bg-secondary me-1 mb-1">{{ tech }}</span>
                    {% endfor %}
                </div>
                {% endif %}
                
                <p class="card-text">{{ assignment.content | strip_html | truncatewords: 20 }}</p>
            </div>
            <div class="card-footer bg-transparent">
                <a href="{{ assignment.url | relative_url }}" class="btn btn-primary">
                    View Assignment <i class="fas fa-arrow-right ms-1"></i>
                </a>
                {% if assignment.rubric %}
                <a href="{{ assignment.rubric | relative_url }}" class="btn btn-outline-secondary ms-2">
                    <i class="fas fa-clipboard-check me-1"></i>Rubric
                </a>
                {% endif %}
            </div>
        </div>
    </div>
    {% endfor %}
</div>

<div class="row mt-5">
    <div class="col-lg-8">
        <h3>Assignment Timeline</h3>
        <div class="timeline">
            {% assign assignments = site.assignments | sort: 'order' %}
            {% for assignment in assignments %}
            <div class="timeline-item mb-3">
                <div class="card">
                    <div class="card-body">
                        <h6 class="card-title">{{ assignment.title }}</h6>
                        {% if assignment.due_date %}
                        <small class="text-muted">Due: {{ assignment.due_date }}</small>
                        {% endif %}
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
    </div>
    <div class="col-lg-4">
        <h3>Quick Links</h3>
        <div class="list-group">
            <a href="{{ '/resources/' | relative_url }}" class="list-group-item list-group-item-action">
                <i class="fas fa-tools me-2"></i>Development Resources
            </a>
            <a href="{{ '/lessons/' | relative_url }}" class="list-group-item list-group-item-action">
                <i class="fas fa-book me-2"></i>Course Lessons
            </a>
            <a href="{{ '/syllabus/' | relative_url }}" class="list-group-item list-group-item-action">
                <i class="fas fa-file-text me-2"></i>Course Syllabus
            </a>
        </div>
    </div>
</div>
