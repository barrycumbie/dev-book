---
layout: default
title: Syllabus
permalink: /syllabus/
---

<div class="hero-section bg-primary text-white p-4 rounded mb-4">
    <div class="row align-items-center">
        <div class="col-lg-8">
            <h1 class="mb-3">📘 CIS 376 Syllabus</h1>
            <p class="lead mb-0">{{ site.course.name }} • {{ site.course.term }}</p>
        </div>
        <div class="col-lg-4 text-center">
            <i class="fas fa-graduation-cap display-3 opacity-50"></i>
        </div>
    </div>
</div>

<div class="row">
    <div class="col-lg-8">
        <h2>Course Information</h2>
        <div class="card mb-4">
            <div class="card-body">
                <div class="row">
                    <div class="col-md-6">
                        <p><strong>Instructor:</strong> {{ site.author }}</p>
                        <p><strong>Email:</strong> <a href="mailto:{{ site.email }}">{{ site.email }}</a></p>
                        <p><strong>Meeting Times:</strong> {{ site.course.meeting_times }}</p>
                    </div>
                    <div class="col-md-6">
                        <p><strong>Term:</strong> {{ site.course.term }}</p>
                        <p><strong>Office Hours:</strong> <em>TBD</em> (posted in Canvas)</p>
                        <p><strong>Term Dates:</strong> {{ site.course.start_date }} – {{ site.course.end_date }}</p>
                    </div>
                </div>
            </div>
        </div>

        <h2>Key Dates</h2>
        <div class="row mb-4">
            <div class="col-md-6">
                <ul class="list-group">
                    <li class="list-group-item d-flex justify-content-between">
                        <span>Add/Drop Deadline</span>
                        <strong>Aug 27</strong>
                    </li>
                    <li class="list-group-item d-flex justify-content-between">
                        <span>Midterm Exam</span>
                        <strong>Oct 9</strong>
                    </li>
                    <li class="list-group-item d-flex justify-content-between">
                        <span>Last Day to Withdraw</span>
                        <strong>Nov 24</strong>
                    </li>
                </ul>
            </div>
            <div class="col-md-6">
                <ul class="list-group">
                    <li class="list-group-item d-flex justify-content-between">
                        <span>Finals Week</span>
                        <strong>Dec 5–10</strong>
                    </li>
                    <li class="list-group-item d-flex justify-content-between">
                        <span>Classes End</span>
                        <strong>Dec 10</strong>
                    </li>
                </ul>
            </div>
        </div>

        <h2>Course Overview</h2>
        <p>
            CIS 376 Web Development introduces students to front-end web development technologies and practices. 
            Students will learn HTML5, CSS3, JavaScript, and modern development workflows while building 
            professional-quality web applications.
        </p>

        <h3>Learning Objectives</h3>
        <ul>
            <li>Master HTML5 semantic markup and accessibility principles</li>
            <li>Create responsive layouts using CSS3 and Bootstrap framework</li>
            <li>Implement interactive functionality with JavaScript and DOM manipulation</li>
            <li>Develop professional development workflows using Git and GitHub</li>
            <li>Deploy static websites using GitHub Pages</li>
            <li>Apply web development best practices and industry standards</li>
        </ul>

        <h2>Grading Overview</h2>
        <div class="table-responsive">
            <table class="table table-striped">
                <thead>
                    <tr>
                        <th>Component</th>
                        <th>Quantity</th>
                        <th>Points Each</th>
                        <th>Total Points</th>
                        <th>Percentage</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Major Projects (Alpha, Bravo, Charlie)</td>
                        <td>3</td>
                        <td>100</td>
                        <td>300</td>
                        <td>60%</td>
                    </tr>
                    <tr>
                        <td>Midterm Exam</td>
                        <td>1</td>
                        <td>75</td>
                        <td>75</td>
                        <td>15%</td>
                    </tr>
                    <tr>
                        <td>Final Exam</td>
                        <td>1</td>
                        <td>75</td>
                        <td>75</td>
                        <td>15%</td>
                    </tr>
                    <tr>
                        <td>Small Assignments & CodeAcademy</td>
                        <td>Various</td>
                        <td>-</td>
                        <td>50</td>
                        <td>10%</td>
                    </tr>
                </tbody>
                <tfoot>
                    <tr class="table-primary">
                        <th>Total</th>
                        <th>-</th>
                        <th>-</th>
                        <th>500</th>
                        <th>100%</th>
                    </tr>
                </tfoot>
            </table>
        </div>

        <h3>Grading Scale</h3>
        <div class="row">
            <div class="col-md-6">
                <ul class="list-group">
                    <li class="list-group-item d-flex justify-content-between">
                        <span>A</span>
                        <span>90-100%</span>
                    </li>
                    <li class="list-group-item d-flex justify-content-between">
                        <span>B</span>
                        <span>80-89%</span>
                    </li>
                    <li class="list-group-item d-flex justify-content-between">
                        <span>C</span>
                        <span>70-79%</span>
                    </li>
                </ul>
            </div>
            <div class="col-md-6">
                <ul class="list-group">
                    <li class="list-group-item d-flex justify-content-between">
                        <span>D</span>
                        <span>60-69%</span>
                    </li>
                    <li class="list-group-item d-flex justify-content-between">
                        <span>F</span>
                        <span>Below 60%</span>
                    </li>
                </ul>
            </div>
        </div>
    </div>

    <div class="col-lg-4">
        <div class="card mb-4">
            <div class="card-header">
                <h5 class="mb-0">Quick Navigation</h5>
            </div>
            <div class="card-body">
                <div class="d-grid gap-2">
                    <a href="{{ '/syllabus/policies' | relative_url }}" class="btn btn-outline-primary">
                        <i class="fas fa-gavel me-2"></i>Course Policies
                    </a>
                    <a href="{{ '/calendar/fall-2025-calendar' | relative_url }}" class="btn btn-outline-primary">
                        <i class="fas fa-calendar me-2"></i>Course Calendar
                    </a>
                    <a href="{{ '/assignments/' | relative_url }}" class="btn btn-outline-primary">
                        <i class="fas fa-tasks me-2"></i>Assignments
                    </a>
                    <a href="{{ '/resources/' | relative_url }}" class="btn btn-outline-primary">
                        <i class="fas fa-tools me-2"></i>Resources
                    </a>
                </div>
            </div>
        </div>

        <div class="card">
            <div class="card-header">
                <h5 class="mb-0">Important Links</h5>
            </div>
            <div class="card-body">
                <ul class="list-unstyled">
                    <li><a href="https://canvas.una.edu" target="_blank">Canvas LMS</a></li>
                    <li><a href="https://github.com" target="_blank">GitHub</a></li>
                    <li><a href="https://www.codecademy.com" target="_blank">Codecademy</a></li>
                    <li><a href="https://validator.w3.org/nu/" target="_blank">Nu HTML Validator</a></li>
                    <li><a href="https://wave.webaim.org/" target="_blank">WAVE Accessibility</a></li>
                </ul>
            </div>
        </div>
    </div>
</div>
