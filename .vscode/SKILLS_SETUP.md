# VS Code + GitHub Copilot Skills Setup for numbers-parser

This guide helps you set up and use GitHub Copilot Skills, including the `ui-ux-pro-max-skill`, in VS Code when working on the numbers-parser project.

## Quick Start

### 1. Install Required Extensions

Install these VS Code extensions:

1. **GitHub Copilot** - AI pair programmer
   - Extension ID: `GitHub.copilot`
   - [Install from Marketplace](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot)

2. **GitHub Copilot Chat** - Chat interface for Copilot
   - Extension ID: `GitHub.copilot-chat`
   - [Install from Marketplace](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot-chat)

3. **Roo Code** (Optional) - If you prefer Roo Code interface
   - Search for "Roo Code" in the VS Code marketplace

### 2. Verify Your Setup

After installing the extensions:

1. Open Command Palette: `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows/Linux)
2. Type "GitHub Copilot: Sign In" and sign in with your GitHub account
3. Verify Copilot is active by looking for the Copilot icon in the status bar

### 3. Open Copilot Chat

To start using skills:

- Press `Cmd+I` (Mac) or `Ctrl+I` (Windows/Linux) to open inline chat
- Or press `Cmd+Shift+I` to open the chat panel
- Or click the chat icon in the activity bar

## Using ui-ux-pro-max-skill

The `ui-ux-pro-max-skill` is designed to help with UI/UX improvements to documentation and code examples.

### Basic Usage

In the Copilot Chat, type prompts like:

```
@workspace How can I improve the user experience of the README?
```

```
Can you analyze the documentation structure and suggest improvements?
```

```
Help me make the installation instructions more user-friendly
```

### Specific to numbers-parser

Try these prompts for this project:

#### Improve Documentation
```
@workspace #file:README.md Can you suggest ways to make the Quick Start section more intuitive?
```

```
How can I improve the API documentation to make it easier for beginners to understand?
```

#### Enhance Code Examples
```
Can you add more practical examples to show how to work with Numbers files?
```

```
Help me create a tutorial-style example that walks through common tasks
```

#### Better Error Messages
```
@workspace Can you review the error handling in the library and suggest more user-friendly error messages?
```

## VS Code Settings for This Project

The `.vscode/settings.json` file in this repository is already configured with recommended settings for Python development. It includes:

- Python formatting with Black
- Code organization with imports
- Testing with pytest
- Linting with Ruff

These settings work seamlessly with GitHub Copilot to provide consistent code suggestions.

## Working with Roo Code

If you're using Roo Code:

### Activation

1. Open the Roo Code panel (usually in the sidebar)
2. Click "New Chat" or use the command palette
3. Start typing your request

### Roo Code Tips

- **Be conversational**: Roo Code works well with natural language
- **Iterate**: Start with a general request, then refine
- **Use context**: Mention file names and specific sections

Example conversation:
```
You: I want to improve the README.md file
Roo: I can help! What specific aspect would you like to improve?
You: Make the installation instructions clearer for Windows users
Roo: [Provides suggestions and can implement changes]
```

## Keyboard Shortcuts

Useful shortcuts when working with Copilot Skills:

| Action | Mac | Windows/Linux |
|--------|-----|---------------|
| Open Inline Chat | `Cmd+I` | `Ctrl+I` |
| Open Chat Panel | `Cmd+Shift+I` | `Ctrl+Shift+I` |
| Accept Suggestion | `Tab` | `Tab` |
| Reject Suggestion | `Esc` | `Esc` |
| Next Suggestion | `Option+]` | `Alt+]` |
| Previous Suggestion | `Option+[` | `Alt+[` |

## Best Practices

### 1. Provide Context

Always give Copilot enough context:

**Bad:**
```
Improve this
```

**Good:**
```
@workspace #file:README.md Improve the installation section for Windows users
who are not familiar with Python package management
```

### 2. Be Specific About UI/UX Goals

**Bad:**
```
Make the docs better
```

**Good:**
```
Make the documentation more scannable by adding:
- More section headings
- Code examples for each feature
- A table of contents
```

### 3. Iterate and Refine

Start broad, then narrow down:

1. "Analyze the user experience of the README"
2. Review suggestions
3. "Now focus on improving the Quick Start section"
4. Review and implement

### 4. Use Workspace Context

The `@workspace` agent understands your entire project:

```
@workspace Find all the places where we explain cell formatting and make them consistent
```

## Common UI/UX Tasks for This Project

### Task 1: Improve Documentation Structure

```
@workspace Can you analyze the README.md structure and suggest how to reorganize
it to be more user-friendly? Consider the different user personas: beginners,
intermediate Python developers, and advanced users.
```

### Task 2: Better Code Examples

```
@workspace #file:README.md The code examples are good, but can you suggest
additional examples that show common real-world use cases for the numbers-parser
library?
```

### Task 3: Enhanced API Documentation

```
@workspace How can we improve the API documentation in the docs folder to make
it more accessible? Consider adding more examples and clearer descriptions.
```

### Task 4: User Onboarding

```
Can you help me create a GETTING_STARTED.md file that provides a step-by-step
tutorial for new users of numbers-parser?
```

## Troubleshooting

### Copilot Not Responding

1. Check the Copilot icon in the status bar - it should show as active
2. Try signing out and signing back in
3. Restart VS Code
4. Check your internet connection

### Suggestions Not Relevant

1. Provide more context in your prompt
2. Specify the file you're working on with `#file:`
3. Use `@workspace` to give broader context
4. Be more specific about what you want

### Roo Code Not Available

1. Verify the extension is installed and enabled
2. Check if your Copilot subscription includes Roo Code access
3. Try the standard Copilot Chat instead

## Learning Resources

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [VS Code Copilot Guide](https://code.visualstudio.com/docs/editor/github-copilot)
- [Copilot Chat Documentation](https://docs.github.com/en/copilot/github-copilot-chat)
- [Main Skills Documentation](../COPILOT_SKILLS.md)

## Getting Help

If you have questions about using Copilot Skills with this project:

1. Check the [main skills documentation](../COPILOT_SKILLS.md)
2. Read the [README](../README.md) for project-specific information
3. Open an issue on the [repository](https://github.com/daddytigerflying/numbers-parser)

---

**Remember**: GitHub Copilot Skills are tools to help you work more efficiently. They work best when you provide clear context and specific goals. Don't hesitate to iterate and refine your prompts!
