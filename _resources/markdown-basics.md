---
title: "📄 Markdown Basics"
subtitle: "GitHub-Flavored Markdown essentials"
layout: resource
category: "documentation"
order: 2
---

## What is Markdown?
Markdown is a lightweight markup language that allows you to format text using simple syntax. GitHub uses a variant called **GitHub-Flavored Markdown (GFM)** that includes additional features.

## Basic Syntax

### Headers
```markdown
# H1 Header
## H2 Header
### H3 Header
#### H4 Header
##### H5 Header
###### H6 Header
```

### Text Formatting
```markdown
**Bold text**
*Italic text*
***Bold and italic***
~~Strikethrough~~
`Inline code`
```

### Lists
```markdown
Unordered list:
- Item 1
- Item 2
  - Sub-item A
  - Sub-item B

Ordered list:
1. First item
2. Second item
3. Third item
```

### Links and Images
```markdown
[Link text](https://example.com)
[Link with title](https://example.com "Optional title")

![Alt text](image-url.jpg)
![Alt text](image-url.jpg "Optional title")
```

## Code Blocks
Use fenced code blocks with language specification for syntax highlighting:

```markdown
```js
console.log("Hello, Markdown!");
```
```

```markdown
```html
<div class="container">
    <h1>Hello World</h1>
</div>
```
```

```markdown
```css
.container {
    max-width: 1200px;
    margin: 0 auto;
}
```
```

## Tables
```markdown
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Row 1    | Data     | More     |
| Row 2    | Data     | More     |
```

## GitHub-Specific Features

### Task Lists
```markdown
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task
```

### Emoji
```markdown
:smile: :heart: :thumbsup: :rocket:
```

### Mentions and References
```markdown
@username
#123 (issue reference)
SHA: a5c3785ed8d6a35868bc169f07e40e889087fd2e
```

## README Best Practices
- Keep it concise and helpful
- Include project description
- Add installation instructions
- Provide usage examples
- Include contribution guidelines
- Add license information

## Example README Structure
```markdown
# Project Title

Brief description of your project.

## Installation
Steps to install and set up the project.

## Usage
How to use the project with examples.

## Contributing
Guidelines for contributing to the project.

## License
License information.
```
