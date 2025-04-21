# Writing Space

A minimalist text editor with rich formatting capabilities in a clean, dark-themed interface.

## Features

### Text Formatting
- **Basic Formatting**: Bold, italic, and underline text
- **Lists**: Ordered (numbered) and unordered (bullet) lists with multi-level support
- **Headings**: Two heading styles (H1 and H2)

### Editor Functions
- **History Management**: Undo and redo actions
- **Clipboard Support**: Copy selected text or all content
- **Text Management**: Clear all text with a single click

### Smart Features
- **Auto-List Detection**: Type "1. " to automatically create a numbered list
- **Bullet List Conversion**: Type "• " to automatically create a bullet list
- **List Indentation**: Use Tab key to indent list items and Shift+Tab to outdent
- **Context-Aware Formatting**: Headings have restricted formatting options

### Keyboard Shortcuts
- **Ctrl+Z**: Undo last action
- **Ctrl+Y** or **Ctrl+Shift+Z**: Redo last undone action
- **Shift+Enter**: Insert line break without creating a new paragraph
- **Tab/Shift+Tab**: Indent/outdent list items

## Usage

Simply open the HTML file in a web browser to start using the editor. The toolbar at the top provides access to all formatting options.

### Working with Lists
- Create lists by clicking the numbered or bullet list buttons
- Indent items by pressing Tab when the cursor is in a list item
- Outdent items by pressing Shift+Tab
- Lists will automatically maintain proper nesting styles (numbers, letters)

### Working with Headings
- Apply headings by selecting the H1 or H2 button
- Heading formatting is exclusive - when text is formatted as a heading, other formatting options are disabled

### Using the Clipboard
- Select specific text to copy only that selection
- Click the copy button without a selection to copy all text

## Technical Details

This editor is built with plain HTML, CSS, and JavaScript with:
- Contenteditable div as the editing surface
- Custom formatting logic using document.execCommand()
- Event listeners for keyboard shortcuts and selection changes
- Special handling for list indentation and heading formats
- CSS for consistent styling across modern browsers

## Browser Compatibility

The editor works in all modern browsers but relies on the document.execCommand() API, which is deprecated though still widely supported.

The following browsers are fully supported:
- Chrome
- Firefox
- Edge
- Safari

## File Structure

The entire application is contained in a single HTML file with:
- Inline CSS for styling
- Embedded JavaScript for editor functionality
- External image resources for toolbar icons
