# RegEx Text Search

A command-line tool for learning and testing Regular Expressions (RegEx) with real-time visual feedback and colored highlighting.

## Overview

RegEx Text Search is an interactive C++ application that helps users understand and test regular expressions by providing immediate visual feedback. The program highlights matched patterns in your text, displays match counts, and includes a comprehensive regex cheat sheet for quick reference.

## Features

- **Interactive Text Search**: Enter custom text and test regex patterns against it in real-time
- **Visual Highlighting**: Matched patterns are highlighted with colored backgrounds for easy identification
- **Regex Validation**: Built-in validation to catch and handle invalid regular expressions
- **Comprehensive Cheat Sheet**: Displays a complete regex reference guide including:
  - Character classes (`\w`, `\d`, `\s`)
  - Anchors (`^`, `$`, `\b`)
  - Groups and lookarounds
  - Quantifiers (`*`, `+`, `?`, `{n}`)
  - Escaped characters
- **Dynamic Updates**: Modify text or regex patterns on-the-fly without restarting
- **Match Counter**: Shows the total number of matches found
- **Colored Terminal Output**: Enhanced readability with ANSI color codes
- **Typing Effects**: Visual feedback with animated text displays

## Usage

### Building the Project

The project includes a makefile for easy compilation:

```bash
make
```

### Running the Application

After building, run the executable:

```bash
./regex-search
```

### Workflow

1. **Initial Setup**
   - The program displays a regex cheat sheet
   - Enter your text to search within
   - Enter a regular expression pattern

2. **View Results**
   - Matched patterns are highlighted in blue
   - Total match count is displayed in green (or red if no matches)
   - The current regex expression is shown

3. **Interactive Menu**
   - Option 1: Change the input text
   - Option 2: Change the regular expression
   - Option 3: Exit the program

4. **Error Handling**
   - Invalid regex patterns trigger an error message
   - Options to re-enter text, regex, or exit
   - Empty inputs are rejected with helpful prompts

## Project Structure

```
regex-text-search/
├── main.cpp          # Entry point and main program loop
├── helpers.cpp       # Input validation and regex application logic
├── helpers.h         # Helper function declarations
├── messages.cpp      # UI display functions and cheat sheet
├── messages.h        # Message function declarations
├── colors.cpp        # ANSI color code implementations
├── colors.h          # Color constant definitions
└── makefile          # Build configuration
```

## Technical Details

- **Language**: C++
- **Key Libraries**: 
  - `<regex>` for pattern matching
  - `<iostream>` for I/O operations
  - `<unistd.h>` for sleep/timing effects
- **Platform**: Unix-based systems (uses `system("clear")` and ANSI colors)

## Example Use Cases

- Learning regex syntax with immediate feedback
- Testing patterns before implementing them in production code
- Validating data extraction patterns
- Experimenting with complex regex expressions
- Teaching regular expressions to beginners

## Authors

Built by Lamia and Abbas (BCS-4C), Dr. Nasir Uddin's students

## License

This project is available for educational purposes.