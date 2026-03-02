# Simple Calculator

## Architecture
- Tier 1 static site — single `index.html` with inline CSS and JS
- No frameworks, no build tools, no dependencies

## Features
- Number buttons (0-9), decimal point
- Operations: +, −, ×, ÷, parentheses
- Equals (=) computes result, Clear (C) resets
- Proper order of operations via recursive descent parser
- Division by zero shows "Error"
- Keyboard support (digits, operators, Enter, Escape, Backspace)
- Responsive design (max-width 320px, scales on mobile)

## Key Decisions
- Used recursive descent parser (parseExpr → parseTerm → parseFactor) for correct operator precedence instead of eval()
- Dark theme with pink/purple accent colors for modern look
- Expression shown above result for context
