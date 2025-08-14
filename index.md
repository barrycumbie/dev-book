---
layout: default
title: CIS 376 Web Development
---

<div class="hero-section bg-primary text-white p-5 rounded mb-5">
    <div class="container">
        <div class="row align-items-center">
            <div class="col-lg-8">
                <h1 class="display-4 fw-bold mb-3">
                    <i class="fas fa-code me-3"></i>CIS 376 — Web Development
                </h1>
                <p class="lead mb-4">Front End Development • Fall 2025</p>
                <p class="mb-4">
                    Welcome! This space hosts student-facing materials for CIS 376. 
                    Start with <strong>Onboarding</strong>, then work through Projects 
                    <strong>Alpha</strong>, <strong>Bravo</strong>, and <strong>Charlie</strong>, 
                    with quizzes and exams in between.
                </p>
                <a href="{{ '/assignments/onboarding' | relative_url }}" class="btn btn-light btn-lg">
                    <i class="fas fa-rocket me-2"></i>Get Started
                </a>
            </div>
            <div class="col-lg-4 text-center">
                <i class="fas fa-laptop-code display-1 opacity-50"></i>
            </div>
        </div>
    </div>
</div>

<div class="row">
    <div class="col-lg-4 mb-4">
        <div class="card h-100">
            <div class="card-body">
                <h5 class="card-title">
                    <i class="fas fa-info-circle text-primary me-2"></i>Course Info
                </h5>
                <ul class="list-unstyled">
                    <li><strong>Instructor:</strong> {{ site.author }}</li>
                    <li><strong>Email:</strong> <a href="mailto:{{ site.email }}">{{ site.email }}</a></li>
                    <li><strong>Term:</strong> {{ site.course.term }}</li>
                    <li><strong>Meeting:</strong> {{ site.course.meeting_times }}</li>
                    <li><strong>Total Class Days:</strong> 30</li>
                    <li><strong>Working Days:</strong> 72</li>
                </ul>
                <a href="{{ '/syllabus' | relative_url }}" class="btn btn-outline-primary">
                    View Full Syllabus
                </a>
            </div>
        </div>
    </div>

    <div class="col-lg-4 mb-4">
        <div class="card h-100">
            <div class="card-body">
                <h5 class="card-title">
                    <i class="fas fa-tasks text-success me-2"></i>Major Projects
                </h5>
                <div class="list-group list-group-flush">
                    <a href="{{ '/assignments/project-alpha' | relative_url }}" 
                       class="list-group-item list-group-item-action">
                        <div class="d-flex w-100 justify-content-between">
                            <h6 class="mb-1">🇦 Project Alpha</h6>
                            <small>100 pts</small>
                        </div>
                        <p class="mb-1">Developer Profile Site</p>
                    </a>
                    <a href="{{ '/assignments/project-bravo' | relative_url }}" 
                       class="list-group-item list-group-item-action">
                        <div class="d-flex w-100 justify-content-between">
                            <h6 class="mb-1">🇧 Project Bravo</h6>
                            <small>100 pts</small>
                        </div>
                        <p class="mb-1">Interactive Web Game</p>
                    </a>
                    <a href="{{ '/assignments/project-charlie' | relative_url }}" 
                       class="list-group-item list-group-item-action">
                        <div class="d-flex w-100 justify-content-between">
                            <h6 class="mb-1">🇨 Project Charlie</h6>
                            <small>100 pts</small>
                        </div>
                        <p class="mb-1">Blog + Data Integration</p>
                    </a>
                </div>
            </div>
        </div>
    </div>

    <div class="col-lg-4 mb-4">
        <div class="card h-100">
            <div class="card-body">
                <h5 class="card-title">
                    <i class="fas fa-calendar-alt text-warning me-2"></i>Key Dates
                </h5>
                <ul class="list-unstyled">
                    <li><strong>Classes Start:</strong> Aug 20</li>
                    <li><strong>Add/Drop Ends:</strong> Aug 27</li>
                    <li><strong>Midterm Exam:</strong> Oct 9</li>
                    <li><strong>Last Withdraw:</strong> Nov 24</li>
                    <li><strong>Finals Week:</strong> Dec 5–10</li>
                    <li><strong>Classes End:</strong> Dec 10</li>
                </ul>
                <a href="{{ '/calendar/fall-2025-calendar' | relative_url }}" class="btn btn-outline-warning">
                    View Full Calendar
                </a>
            </div>
        </div>
    </div>
</div>

<div class="row mt-4">
    <div class="col-lg-6 mb-4">
        <div class="card">
            <div class="card-body">
                <h5 class="card-title">
                    <i class="fas fa-graduation-cap text-info me-2"></i>Quick Links
                </h5>
                <div class="row">
                    <div class="col-6">
                        <a href="{{ '/assignments' | relative_url }}" class="btn btn-sm btn-outline-primary w-100 mb-2">
                            Assignments
                        </a>
                        <a href="{{ '/resources' | relative_url }}" class="btn btn-sm btn-outline-primary w-100 mb-2">
                            Resources
                        </a>
                    </div>
                    <div class="col-6">
                        <a href="{{ '/exams' | relative_url }}" class="btn btn-sm btn-outline-primary w-100 mb-2">
                            Exams
                        </a>
                        <a href="{{ '/lessons' | relative_url }}" class="btn btn-sm btn-outline-primary w-100 mb-2">
                            Lessons
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="col-lg-6 mb-4">
        <div class="card">
            <div class="card-body">
                <h5 class="card-title">
                    <i class="fas fa-tools text-secondary me-2"></i>Essential Resources
                </h5>
                <ul class="list-unstyled">
                    <li><a href="{{ '/resources/vs-code-tips' | relative_url }}">VS Code Tips & Tricks</a></li>
                    <li><a href="{{ '/resources/markdown-basics' | relative_url }}">Markdown Basics</a></li>
                    <li><a href="{{ '/resources/keyboard-shortcuts' | relative_url }}">Keyboard Shortcuts</a></li>
                    <li><a href="{{ '/resources/nato-phonetic' | relative_url }}">NATO Phonetic Reference</a></li>
                    <li><a href="{{ '/resources/ergonomics' | relative_url }}">Ergonomics & Well-Being</a></li>
                </ul>
            </div>
        </div>
    </div>
</div>
