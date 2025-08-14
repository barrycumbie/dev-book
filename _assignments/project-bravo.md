---
title: "🇧 Project Bravo — Web Game"
subtitle: "Build an interactive web-based game"
layout: assignment
points: 100
due_date: "End of Week 6"
submit_format: "Repo URL (Pages deployed)"
difficulty: 4
technologies:
  - JavaScript
  - DOM Manipulation
  - Arrays & Objects
  - Event Handling
  - Bootstrap/jQuery UI
  - GitHub Pages
objectives:
  - Implement complex DOM manipulation
  - Work with arrays and objects for game data
  - Handle user events and interactions
  - Create engaging user interfaces
  - Apply randomization and game logic
rubric: "/assignments/rubrics/bravo-rubric"
order: 3
---

## 📌 Overview
Build a small **web game** (matching/drag/flip/memory/quiz). Use arrays/objects, randomization, events, and track player progress with a polished user interface.

## 🎯 Objectives
- DOM manipulation in response to user **events**
- **Array of objects** for game data + **randomization**
- UI polish (Bootstrap/jQuery UI) and clear instructions
- Game state management and progress tracking

## 🧭 Requirements

### Game Options
Choose one of these game types (or propose your own):
- **Memory/Matching Game** - Flip cards to find pairs
- **Drag & Drop Puzzle** - Arrange pieces to complete an image
- **Quiz Game** - Multiple choice with scoring and feedback
- **Word Game** - Hangman, word scramble, or similar
- **Simple Arcade** - Snake, Tetris-style, or reaction game

### Technical Requirements

#### Core Functionality
- **User greeting** and name collection
- **Clear instructions** displayed prominently
- **Progress tracking** (score, lives, level, etc.)
- **Reset/restart** functionality
- **Randomization** of game elements
- **Win/lose conditions** with appropriate feedback

#### Data Structure
- Use **arrays of objects** to store game data
- Implement proper data organization
- Handle game state effectively

#### User Interface
- Responsive design using Bootstrap
- At least **one UI enhancement**:
  - Drag and drop functionality
  - Card flip animations
  - Modal dialogs
  - Progress bars
  - Sound effects
  - Particle effects
- Clear visual feedback for user actions
- Professional styling and layout

#### Code Quality
- Well-organized JavaScript functions
- Proper event handling
- Error handling and validation
- Comprehensive comments
- Clean, readable code structure

### Project Structure
```
project-bravo/
├── index.html
├── README.md
├── scripts/
│   ├── game.js
│   ├── data.js
│   └── ui.js
├── styles/
│   └── game.css
├── images/
│   ├── wireframe.png
│   ├── screenshot.png
│   └── game-assets/
└── sounds/ (optional)
    └── game-sounds/
```

### Documentation
- **Wireframe** saved in `/images` and linked in README
- **Screenshot** of completed game
- Comprehensive README including:
  - Game description and rules
  - Technologies used
  - Setup instructions
  - Credits for any assets used

### Integration
- **Footer links** to:
  - Your Dev Profile (Project Alpha)
  - Source code repository
  - Nu HTML Validator results
  - WAVE accessibility results
- **Update Dev Profile** with:
  - Screenshot of the game
  - Link to live game
  - Brief description in projects section

## 📑 Submission Checklist
- [ ] Repository is public
- [ ] GitHub Pages is live and functional
- [ ] Game works without errors
- [ ] README is complete with all required information
- [ ] Wireframe is uploaded and linked
- [ ] Screenshot is included
- [ ] All footer validation links work
- [ ] Dev Profile is updated with game link
- [ ] Game includes all required functionality
- [ ] UI enhancement is implemented
- [ ] Code is well-commented and organized

## 💡 Game Ideas & Inspiration

### Memory Game
- Grid of cards that flip to reveal images
- Player finds matching pairs
- Track time and number of moves
- Multiple difficulty levels

### Drag & Drop Puzzle
- Image split into pieces
- Player drags pieces to correct positions
- Snap-to-grid functionality
- Progress indicator

### Quiz Game
- Multiple choice questions
- Score tracking
- Timer (optional)
- Question randomization
- Feedback for correct/incorrect answers

### Word Game
- Hangman with visual gallows
- Word scramble with hints
- Letter guessing with alphabet display
- Category-based words

## 🎨 UI Enhancement Ideas
- **Animations**: CSS transitions, keyframes
- **Drag & Drop**: HTML5 drag API or library
- **Modals**: Bootstrap modals for instructions/results
- **Progress Bars**: Visual progress indicators
- **Sound Effects**: Audio feedback for actions
- **Particle Effects**: Celebration animations
- **Responsive Gestures**: Touch/swipe on mobile

## 📊 Rubric
See [Bravo Rubric]({{ page.rubric | relative_url }}) for detailed grading criteria.

## 🔗 Helpful Resources
- [JavaScript Array Methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
- [DOM Event Handling](https://developer.mozilla.org/en-US/docs/Web/API/Event)
- [CSS Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations)
- [Bootstrap Components](https://getbootstrap.com/docs/5.0/components/)
- [HTML5 Drag and Drop](https://developer.mozilla.org/en-US/docs/Web/API/HTML_Drag_and_Drop_API)
