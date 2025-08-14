---
title: "🇨 Project Charlie — Full-Stack Web App"
subtitle: "Build a complete web application with database"
layout: default
parent: Assignments
nav_order: 4
points: 100
due_date: "End of Week 9"
submit_format: "Link to Dev Profile (links out to Admin & Data)"
difficulty: 5
technologies:
  - JSON
  - Fetch API
  - CRUD Operations
  - GitHub Pages
  - Data Management
  - RESTful Concepts
objectives:
  - Separate data from presentation
  - Implement fetch API for data retrieval
  - Create administrative interface
  - Understand JSON data structures
  - Practice API integration patterns
rubric: "{% link _assignments/charlie-rubric.md %}"
order: 4
---

## 📌 Overview
Create a sophisticated blog system by splitting functionality across three repositories:
- **Data Repository** - JSON data served via GitHub Pages
- **Blog Admin** - Administrative interface for managing posts
- **Developer Profile** - Updated to fetch and display blog data

This project demonstrates real-world patterns of separating data, administration, and presentation layers.

## 🧭 Project Architecture

### Three-Repository Structure
1. **Data Repository** (`project-charlie-data`)
   - Contains JSON files with blog posts
   - Served via GitHub Pages as a simple API
   - Strict JSON format with validation

2. **Admin Repository** (`project-charlie-admin`) 
   - Administrative interface for blog management
   - Fetch, display, add, edit, delete posts (temporary)
   - Bootstrap 5 components for professional UI

3. **Developer Profile** (Updated from Project Alpha)
   - Fetches JSON data from data repository
   - Displays blog posts dynamically
   - Links to admin interface

## 🎯 Requirements

### Data Repository Requirements
- **JSON Structure**: Consistent post format
  ```json
  {
    "posts": [
      {
        "id": 1,
        "title": "Post Title",
        "date": "2025-08-14",
        "author": "Your Name",
        "excerpt": "Brief description...",
        "content": "Full post content...",
        "tags": ["web-dev", "javascript"],
        "published": true
      }
    ]
  }
  ```
- **README Documentation**: API endpoints and usage
- **Direct JSON Access**: Working GitHub Pages URL
- **Minimum 5 sample posts** with realistic content

### Admin Interface Requirements
- **Data Fetching**: Load posts from JSON API
- **Display Posts**: List view with post previews
- **CRUD Operations** (temporary - not persistent):
  - **Create**: Add new posts via form
  - **Read**: Display individual posts
  - **Update**: Edit existing posts
  - **Delete**: Remove posts from display
- **Bootstrap 5 Components**: 
  - Navigation
  - Forms
  - Cards/Lists
  - Modals (optional)
  - Alerts for user feedback
- **Error Handling**: Graceful handling of fetch failures
- **Responsive Design**: Works on all device sizes

### Developer Profile Integration
- **Fetch Integration**: Pull blog data from JSON API
- **Dynamic Display**: Show recent posts in blog section
- **Admin Link**: Button/link to admin interface
- **Error Handling**: Fallback if API is unavailable
- **Loading States**: Show loading indicators during fetch

### Technical Specifications
- **JSON Validation**: All JSON must be valid
- **Error Handling**: Proper try/catch for async operations
- **Code Organization**: Separate files for different concerns
- **Documentation**: Comments explaining fetch operations
- **Performance**: Efficient data loading and display

## 📁 Project Structure

### Data Repository
```
project-charlie-data/
├── index.html (redirect to JSON)
├── README.md
├── posts.json
├── authors.json (optional)
└── api/
    └── v1/
        └── posts.json
```

### Admin Repository
```
project-charlie-admin/
├── index.html
├── README.md
├── scripts/
│   ├── admin.js
│   ├── api.js
│   └── ui.js
├── styles/
│   └── admin.css
└── images/
    └── wireframe.png
```

## 📑 Submission Process

### Step 1: Data Repository
1. Create public repository
2. Set up GitHub Pages
3. Create valid JSON with sample posts
4. Test direct JSON access
5. Document API in README

### Step 2: Admin Interface
1. Create admin repository
2. Implement fetch from data API
3. Build CRUD interface
4. Style with Bootstrap 5
5. Deploy via GitHub Pages

### Step 3: Profile Integration
1. Update Project Alpha (Dev Profile)
2. Add fetch functionality to blog section
3. Link to admin interface
4. Test integration end-to-end

### Step 4: Documentation
1. Create wireframe for admin interface
2. Update all README files
3. Add validation links to footers
4. Test all live links

## 📑 Submission Checklist
- [ ] Data repository is public with working JSON API
- [ ] Admin interface deployed and functional
- [ ] Developer Profile updated with fetch integration
- [ ] All three repositories linked properly
- [ ] Wireframe created and linked
- [ ] README files complete in all repositories
- [ ] JSON validates successfully
- [ ] Fetch operations work correctly
- [ ] Bootstrap components implemented
- [ ] All validation links work
- [ ] Error handling implemented
- [ ] Responsive design confirmed

## 💡 Development Tips

### JSON Best Practices
- Use consistent property names
- Include metadata (dates, IDs, authors)
- Validate JSON before committing
- Keep file sizes reasonable

### Fetch API Tips
- Always use try/catch blocks
- Check response.ok before parsing
- Provide user feedback during loading
- Cache data when appropriate

### Admin Interface UX
- Clear navigation between functions
- Form validation and feedback
- Confirmation for destructive actions
- Keyboard shortcuts for power users

### Error Handling
- Network failures
- Invalid JSON responses
- Missing data properties
- User input validation

## 🔍 Testing Checklist
- [ ] JSON API accessible via direct URL
- [ ] Admin interface loads without errors
- [ ] All CRUD operations work
- [ ] Profile fetches and displays data
- [ ] Links between repositories work
- [ ] Error handling functions properly
- [ ] Responsive on mobile and desktop
- [ ] Validation tools return clean results

## 📊 Rubric
See [Charlie Rubric]({{ page.rubric | relative_url }}) for detailed grading criteria.

## 🔗 Helpful Resources
- [Fetch API Documentation](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
- [JSON Validation Tools](https://jsonlint.com/)
- [GitHub Pages Setup](https://docs.github.com/en/pages)
- [Bootstrap 5 Forms](https://getbootstrap.com/docs/5.0/forms/overview/)
- [Async/Await in JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Async_await)
