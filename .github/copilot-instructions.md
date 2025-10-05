# Copilot Instructions for AI Agents

## Project Overview
- This is a simple, static web application for form validation, consisting of `index.html`, `main.js`, and `style.css`.
- The main feature is a sign-up form with username, email, and password fields, providing instant validation feedback.
- No build tools, frameworks, or external dependencies (other than FontAwesome for icons and remote images).

## File Structure
- `index.html`: Main HTML file. Contains the form, layout, and references to scripts/styles.
- `main.js`: Handles form validation logic and DOM manipulation. Uses simple functions for element selection and validation feedback.
- `style.css`: All styling, including responsive design and icon positioning.
- `images/`: Contains SVG assets for branding and illustration.

## Key Patterns & Conventions
- **Validation**: All validation is handled in `main.js` using the `engine` function, which updates error messages and icon visibility based on input state.
- **Element Access**: Uses helper functions `id()` and `classes()` for DOM selection.
- **Form Submission**: The form's default submit is prevented; validation is performed on submit.
- **Icons**: FontAwesome icons are used for visual feedback (success/failure) and are toggled via CSS opacity.
- **Error Handling**: Error messages are shown in `.error` divs next to each input.
- **Responsiveness**: Layout adapts for mobile via media queries in `style.css`.

## Developer Workflows
- **No build step**: Open `index.html` directly in a browser to view and test.
- **Debugging**: Use browser dev tools (Console, Elements, Network) for troubleshooting.
- **No tests**: There are no automated tests or test frameworks.
- **No package management**: All dependencies are CDN-based or local assets.

## Project-Specific Guidance
- Keep all logic in `main.js` and all styles in `style.css`.
- When adding new fields, update both the HTML and the validation logic in `main.js` (add to the `engine` calls and error handling arrays).
- Use the same icon and error message pattern for new fields.
- Reference images and icons using relative paths as in the current codebase.
- Maintain the simple, flat structure—avoid introducing frameworks or build tools.

## Examples
- To add a new input (e.g., phone number):
  - Add the input and associated icons/error div in `index.html`.
  - Update `main.js` to include validation for the new field, following the `engine` pattern.
  - Add any necessary styles to `style.css`.

---
For questions about conventions or structure, see the existing code for examples. Keep changes minimal and consistent with the current approach.