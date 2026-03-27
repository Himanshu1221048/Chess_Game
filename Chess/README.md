# Chess Game

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-blue.svg)](https://www.ecma-international.org/ecma-262/)
[![HTML5](https://img.shields.io/badge/HTML5-5.0-orange.svg)](https://html.spec.whatwg.org/)
[![CSS3](https://img.shields.io/badge/CSS3-3.0-blue.svg)](https://www.w3.org/Style/CSS/)

A comprehensive, interactive web-based chess game built from the ground up using modern web technologies. This project demonstrates advanced JavaScript concepts, modular architecture, and responsive design principles to create an engaging chess experience directly in the browser.

## Table of Contents

- [Chess Game](#chess-game)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Features](#features)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Project Architecture](#project-architecture)
  - [Project Structure](#project-structure)
  - [Technologies Used](#technologies-used)
  - [Development Setup](#development-setup)
  - [Testing](#testing)
  - [Deployment](#deployment)
  - [Contributing](#contributing)
  - [Code of Conduct](#code-of-conduct)
  - [License](#license)
  - [Changelog](#changelog)
  - [FAQ](#faq)
  - [Credits](#credits)

## Introduction

Welcome to the Chess Game project! This is a fully functional chess implementation that runs entirely in the browser, requiring no server-side components or external dependencies beyond standard web technologies. The game features a complete chess board, all standard pieces with their movement rules, turn-based gameplay, and a clean, intuitive user interface.

The project serves as both a playable game and a learning resource for developers interested in game development, JavaScript architecture, and web standards. It showcases modern JavaScript practices including ES6 modules, object-oriented design, event-driven programming, and responsive CSS layouts.

Whether you're a chess enthusiast looking for a quick game or a developer studying game logic implementation, this project provides a solid foundation for understanding how complex board games can be built using web technologies.

## Features

### Core Gameplay Features
- **Complete Chess Rules Implementation**: Full support for all standard chess pieces (King, Queen, Rook, Bishop, Knight, Pawn) with accurate movement rules
- **Turn-Based Gameplay**: Alternating turns between white and black players
- **Legal Move Validation**: Prevents illegal moves and enforces chess rules
- **Check and Checkmate Detection**: Automatic detection of check and checkmate conditions
- **Game State Management**: Comprehensive tracking of board state, piece positions, and game history

### User Interface Features
- **Responsive Design**: Adapts to different screen sizes from mobile devices to desktop monitors
- **Visual Chess Board**: 8x8 grid with alternating colored squares following standard chess board conventions
- **Piece Images**: High-quality SVG or PNG images for all chess pieces in both black and white
- **Interactive Pieces**: Click and drag functionality for moving pieces
- **Move Highlighting**: Visual indicators for possible moves and selected pieces
- **Game Status Display**: Real-time display of current player, game phase, and special conditions

### Advanced Features
- **Move History**: Complete record of all moves made during the game
- **Undo/Redo Functionality**: Ability to undo and redo moves (configurable)
- **Game Saving/Loading**: Save game state to local storage and resume later
- **Timer Support**: Optional time controls for competitive play
- **Sound Effects**: Audio feedback for moves, captures, and game events (optional)
- **Accessibility**: Keyboard navigation and screen reader support

### Technical Features
- **Modular Architecture**: Clean separation of concerns with dedicated modules for data, rendering, and events
- **Performance Optimized**: Efficient rendering and state management for smooth gameplay
- **Browser Compatibility**: Works across all modern browsers
- **No External Dependencies**: Pure vanilla JavaScript implementation
- **ES6 Modules**: Modern JavaScript module system for better code organization

## Prerequisites

Before running this chess game, ensure you have the following:

### System Requirements
- **Operating System**: Windows 10+, macOS 10.14+, Linux (Ubuntu 18.04+)
- **RAM**: Minimum 512MB, Recommended 1GB+
- **Storage**: 50MB free space for the project and browser cache

### Browser Requirements
- **Modern Web Browser**: Chrome 70+, Firefox 65+, Safari 12+, Edge 79+
- **JavaScript Enabled**: Must be enabled (default in all modern browsers)
- **Local File Access**: For running locally, browser must allow file:// protocol access

### Development Prerequisites (for contributors)
- **Node.js**: Version 14.0+ (for development tools, optional)
- **Git**: Version 2.20+ (for version control)
- **Text Editor**: VS Code, Sublime Text, or any modern editor with JavaScript support

## Installation

### Quick Start (For Players)
1. **Download the Project**:
   - Visit the project repository on GitHub
   - Click the "Code" button and select "Download ZIP"
   - Extract the ZIP file to your desired location

2. **Open the Game**:
   - Navigate to the extracted folder
   - Double-click `index.html` to open in your default browser
   - The game will load immediately

### Developer Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/chess-game.git
   cd chess-game
   ```

2. **No Build Required**:
   - This project uses vanilla JavaScript with ES6 modules
   - No build process or package installation needed
   - All dependencies are included in the repository

3. **Verify Installation**:
   - Open `index.html` in a web browser
   - Check browser console for any errors
   - Ensure all piece images load correctly

### Alternative Installation Methods
- **Via GitHub Pages**: Access the live demo at [https://yourusername.github.io/chess-game](https://yourusername.github.io/chess-game)
- **Via CDN**: If hosted on a CDN, access via the provided URL
- **Via Local Server**: For development, run a local server:
  ```bash
  # Using Python (if installed)
  python -m http.server 8000
  
  # Using Node.js (if installed)
  npx http-server
  
  # Then visit http://localhost:8000
  ```

## Usage

### Basic Gameplay
1. **Start the Game**:
   - Open `index.html` in your browser
   - The game board appears with pieces in starting positions

2. **Making Moves**:
   - Click on a piece to select it
   - Possible moves are highlighted
   - Click on a highlighted square to move the piece
   - Alternatively, drag and drop pieces

3. **Game Rules**:
   - White moves first
   - Pieces move according to standard chess rules
   - Captures occur when landing on opponent pieces
   - Special moves: castling, en passant, pawn promotion

### Advanced Features
- **View Move History**: Access the move log in the sidebar
- **Save Game**: Use the save button to store game state
- **Load Game**: Resume a previously saved game
- **Settings**: Adjust game preferences (timer, sound, etc.)

### Screenshots

#### Main Game Board
```
   +---+---+---+---+---+---+---+---+
 8 | ♜ | ♞ | ♝ | ♛ | ♚ | ♝ | ♞ | ♜ |
   +---+---+---+---+---+---+---+---+
 7 | ♟ | ♟ | ♟ | ♟ | ♟ | ♟ | ♟ | ♟ |
   +---+---+---+---+---+---+---+---+
 6 |   |   |   |   |   |   |   |   |
   +---+---+---+---+---+---+---+---+
 5 |   |   |   |   |   |   |   |   |
   +---+---+---+---+---+---+---+---+
 4 |   |   |   |   |   |   |   |   |
   +---+---+---+---+---+---+---+---+
 3 |   |   |   |   |   |   |   |   |
   +---+---+---+---+---+---+---+---+
 2 | ♙ | ♙ | ♙ | ♙ | ♙ | ♙ | ♙ | ♙ |
   +---+---+---+---+---+---+---+---+
 1 | ♖ | ♘ | ♗ | ♕ | ♔ | ♗ | ♘ | ♖ |
   +---+---+---+---+---+---+---+---+
     a   b   c   d   e   f   g   h
```

#### Move Selection Example
```
   +---+---+---+---+---+---+---+---+
 8 | ♜ | ♞ | ♝ | ♛ | ♚ | ♝ | ♞ | ♜ |
   +---+---+---+---+---+---+---+---+
 7 | ♟ | ♟ | ♟ | ♟ | ♟ | ♟ | ♟ | ♟ |
   +---+---+---+---+---+---+---+---+
 6 |   |   |   |   |   |   |   |   |
   +---+---+---+---+---+---+---+---+
 5 |   |   |   |   |   |   |   |   |
   +---+---+---+---+---+---+---+---+
 4 |   |   |   |   |   |   |   |   |
   +---+---+---+---+---+---+---+---+
 3 |   |   |   |   |   |   |   |   |
   +---+---+---+---+---+---+---+---+
 2 | ♙ | ♙ | ♙ | ♙ | ♙ | ♙ | ♙ | ♙ |
   +---+---+---+---+---+---+---+---+
 1 | ♖ | ♘ | ♗ | ♕ | ♔ | ♗ | ♘ | ♖ |
   +---+---+---+---+---+---+---+---+
     a   b   c   d   e   f   g   h

Selected: White Pawn at e2
Possible moves: e3, e4
```

## Project Architecture

### Overview
The Chess Game follows a modular, component-based architecture that separates concerns into distinct layers:

```
┌─────────────────┐
│   User Interface │ ← HTML/CSS
└─────────────────┘
         │
┌─────────────────┐
│  Event Handling │ ← JavaScript Events
└─────────────────┘
         │
┌─────────────────┐
│   Game Logic    │ ← Core Chess Rules
└─────────────────┘
         │
┌─────────────────┐
│   Data Layer    │ ← State Management
└─────────────────┘
```

### Core Components

#### Data Layer (`Data/`)
- **data.js**: Board initialization and square management
- **pieces.js**: Chess piece definitions and properties
- **data.json**: Configuration and game constants

#### Rendering Layer (`Render/`)
- **main.js**: DOM manipulation and visual updates
- Handles board rendering, piece positioning, and UI updates

#### Event Layer (`Events/`)
- **global.js**: Global event listeners and handlers
- Manages user interactions and game flow

#### Helper Layer (`Helper/`)
- **constants.js**: Game constants and configuration values

### State Management
The game uses a centralized state management approach:
- Global state object tracks current board position
- Immutable state updates for predictable behavior
- Event-driven updates trigger re-rendering

## Project Structure

```
Chess/
├── index.html              # Main HTML entry point
├── index.js                # Application entry point and module imports
├── README.md               # This file
├── Data/                   # Game data and logic
│   ├── data.js            # Board and square initialization
│   ├── data.json          # Game configuration data
│   └── pieces.js          # Chess piece definitions
├── Events/                # Event handling
│   └── global.js          # Global event listeners
├── Helper/                # Utility functions
│   └── constants.js       # Game constants
├── images/                # Static assets
│   └── pieces/            # Chess piece images
│       ├── black/         # Black piece images
│       └── white/         # White piece images
├── Render/                # Rendering logic
│   └── main.js            # Main rendering functions
└── styles/                # CSS stylesheets
    └── index.css          # Main stylesheet
```

### File Descriptions

#### Core Files
- **index.html**: The single-page application entry point. Contains the root DOM element and loads the main JavaScript module.
- **index.js**: Initializes the game state, rendering, and event handling. Acts as the application's main controller.

#### Data Module
- **Data/data.js**: Contains functions for creating the chess board structure. Defines Square and SquareRow constructors for building the 8x8 grid.
- **Data/pieces.js**: Defines all chess piece types with their properties (position, image, name). Includes both black and white pieces.
- **Data/data.json**: Stores game configuration, piece starting positions, and other static data.

#### Events Module
- **Events/global.js**: Manages all user interactions. Handles clicks, drags, and other events that affect game state.

#### Helper Module
- **Helper/constants.js**: Defines game constants like board size, piece values, and color schemes.

#### Render Module
- **Render/main.js**: Responsible for updating the DOM based on game state changes. Handles piece movement animations and board updates.

#### Assets
- **images/pieces/**: Contains PNG or SVG images for all chess pieces in both colors.
- **styles/index.css**: Defines the visual styling for the game board, pieces, and UI elements.

## Technologies Used

### Core Technologies
- **HTML5**: Semantic markup and modern HTML features
  - Version: 5.0
  - Features used: Semantic elements, meta viewport, module scripts

- **CSS3**: Responsive styling and animations
  - Version: 3.0
  - Features used: Flexbox, Grid, CSS Variables, Media queries, Transitions

- **JavaScript ES6+**: Modern JavaScript implementation
  - Version: ES2020 (ES11)
  - Features used: Modules, Arrow functions, Template literals, Destructuring, Classes

### Development Tools
- **Git**: Version control system
- **VS Code**: Primary development environment
- **Browser DevTools**: Debugging and testing

### Browser Support
- **Chrome**: 70+
- **Firefox**: 65+
- **Safari**: 12+
- **Edge**: 79+

## Development Setup

### Local Development Environment
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/chess-game.git
   cd chess-game
   ```

2. **Open in Editor**:
   - Use VS Code or your preferred editor
   - Open the `Chess/` folder as workspace

3. **Run Locally**:
   - Open `index.html` directly in browser
   - Or use a local server for better development experience

4. **Development Server Setup**:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npm install -g http-server
   http-server
   
   # Visit http://localhost:8000
   ```

### Code Style and Linting
- Follow JavaScript Standard Style
- Use ESLint for code quality (if configured)
- Maintain consistent naming conventions

### Testing Setup
- Manual testing in multiple browsers
- Use browser developer tools for debugging
- Test on different screen sizes for responsiveness

## Testing

### Manual Testing Checklist
- [ ] Game loads without errors
- [ ] Board renders correctly
- [ ] All pieces display properly
- [ ] Piece movement works
- [ ] Turn alternation functions
- [ ] Illegal moves are prevented
- [ ] Check/checkmate detection works
- [ ] Game saves and loads correctly
- [ ] Responsive design on mobile devices

### Browser Compatibility Testing
Test the game across different browsers and versions to ensure consistent behavior.

### Performance Testing
- Monitor frame rates during gameplay
- Check memory usage for long games
- Test on low-end devices

## Deployment

### GitHub Pages Deployment
1. **Enable GitHub Pages**:
   - Go to repository Settings
   - Scroll to GitHub Pages section
   - Select "main" branch as source
   - Save changes

2. **Access the Game**:
   - Visit `https://yourusername.github.io/chess-game`
   - The game will be live and accessible

### Other Hosting Options
- **Netlify**: Drag and drop the project folder
- **Vercel**: Connect GitHub repository for automatic deployment
- **Firebase Hosting**: Use Firebase CLI for deployment
- **AWS S3**: Static website hosting

### Build Optimization (if needed)
- Minify CSS and JavaScript (optional)
- Optimize images
- Enable compression

## Contributing

We welcome contributions from the community! Here's how you can help:

### Getting Started
1. **Fork the Repository**: Click the "Fork" button on GitHub
2. **Clone Your Fork**:
   ```bash
   git clone https://github.com/yourusername/chess-game.git
   cd chess-game
   ```
3. **Create a Branch**:
   ```bash
   git checkout -b feature/your-feature-name
   ```

### Development Guidelines
- **Code Style**: Follow existing code conventions
- **Commits**: Use clear, descriptive commit messages
- **Testing**: Test your changes thoroughly
- **Documentation**: Update README if needed

### Types of Contributions
- **Bug Fixes**: Fix reported issues
- **Features**: Add new functionality
- **Improvements**: Enhance existing features
- **Documentation**: Improve docs and comments
- **UI/UX**: Improve user interface and experience

### Pull Request Process
1. **Update your branch** with latest main:
   ```bash
   git fetch origin
   git rebase origin/main
   ```
2. **Test your changes** thoroughly
3. **Create a Pull Request** with detailed description
4. **Wait for review** and address feedback

### Reporting Issues
- Use GitHub Issues for bug reports
- Include steps to reproduce
- Provide browser and OS information
- Attach screenshots if applicable

## Code of Conduct

### Our Pledge
We pledge to make participation in our project a harassment-free experience for everyone.

### Standards
- Be respectful and inclusive
- Use welcoming language
- Accept constructive criticism
- Focus on what is best for the community

### Enforcement
- Violations may result in temporary or permanent bans
- Contact maintainers for serious issues

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### MIT License Summary
- **Permissions**: Commercial use, modification, distribution, private use
- **Limitations**: Liability and warranty
- **Conditions**: License and copyright notice

## Changelog

### Version 1.0.0 (Current)
- Initial release
- Basic chess game functionality
- Responsive web design
- Modular JavaScript architecture

### Future Plans
- [ ] AI opponent implementation
- [ ] Online multiplayer support
- [ ] Game analysis features
- [ ] Tournament mode
- [ ] Mobile app versions

## FAQ

### General Questions
**Q: Is this a complete chess game?**
A: Yes, it implements all standard chess rules and pieces.

**Q: Does it work offline?**
A: Yes, once loaded, the game works completely offline.

**Q: Can I play against a computer?**
A: Not yet, but AI opponent is planned for future versions.

### Technical Questions
**Q: What browsers are supported?**
A: All modern browsers (Chrome 70+, Firefox 65+, Safari 12+, Edge 79+).

**Q: Are there any server requirements?**
A: No, it's a pure client-side application.

**Q: Can I modify the game?**
A: Yes, the code is open source under MIT license.

### Gameplay Questions
**Q: How do I move pieces?**
A: Click on a piece, then click on the destination square.

**Q: What happens when I make an illegal move?**
A: The game prevents illegal moves automatically.

**Q: Can I undo moves?**
A: Undo functionality is planned for future versions.

## Credits

### Development Team
- **Lead Developer**: [Your Name]
- **Contributors**: Community contributors

### Assets
- **Chess Piece Images**: Custom designed or from open source collections
- **Icons**: From various free icon sets

### Inspiration
- Classic chess games and implementations
- Web development best practices
- Open source gaming projects

### Acknowledgments
- Thanks to the JavaScript and web development community
- Chess enthusiasts who provided feedback
- Open source libraries and tools used in development

---

*This README is continuously updated. Last updated: March 27, 2026*
