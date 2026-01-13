# GitHub Copilot Skills for numbers-parser

This document explains how to use GitHub Copilot Skills, including the `ui-ux-pro-max-skill`, with the numbers-parser repository in VS Code and Roo Code.

## What are GitHub Copilot Skills?

GitHub Copilot Skills are specialized AI capabilities that help you work with code more effectively. They provide context-aware assistance tailored to specific tasks or domains.

## Prerequisites

- **VS Code**: Install [Visual Studio Code](https://code.visualstudio.com/)
- **GitHub Copilot**: You need an active GitHub Copilot subscription
- **Roo Code Extension**: Install from the VS Code marketplace if you're using Roo Code specifically

## Using the ui-ux-pro-max-skill

The `ui-ux-pro-max-skill` is a specialized skill for UI/UX related tasks. Here's how to use it with this repository:

### 1. Enable GitHub Copilot Chat

1. Open VS Code
2. Press `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows/Linux)
3. Type "GitHub Copilot: Open Chat"
4. Or use the shortcut `Cmd+I` (Mac) or `Ctrl+I` (Windows/Linux)

### 2. Invoke the Skill

In the Copilot Chat, you can invoke skills using the `@` symbol or by directly mentioning them:

```
@workspace Can you help me improve the documentation structure?
```

Or specifically for UI/UX tasks:

```
Can you analyze the user experience of the README.md file?
Can you suggest improvements to the documentation layout?
Can you help me make the API examples more user-friendly?
```

### 3. Using with Roo Code

If you're using Roo Code specifically:

1. Open the Roo Code panel in VS Code
2. Use natural language to describe your UI/UX task
3. Reference the skill context by mentioning UI/UX improvements
4. Roo Code will use the appropriate skill to help you

### Example Prompts for numbers-parser

Here are some useful prompts you can try with the UI/UX skill on this repository:

#### Documentation Improvements
```
Can you review the README.md and suggest ways to make it more beginner-friendly?
How can I improve the quick start section to make it easier for new users?
Can you help me organize the API documentation for better readability?
```

#### Code Examples
```
Can you add more detailed examples to the README showing common use cases?
How can I make the pandas integration example more clear?
Can you suggest a better way to present the cell data examples?
```

#### User Experience
```
How can I improve the installation instructions for different platforms?
Can you suggest a better structure for the limitations section?
What would make the command-line scripts section more user-friendly?
```

## Working with the numbers-parser Repository

When using Copilot Skills with this repository, keep in mind:

### Repository Context

The numbers-parser library is a Python package for working with Apple Numbers files. When asking for help:

1. **Specify the user perspective**: Are you helping end users, contributors, or API users?
2. **Reference existing patterns**: The README already has good examples - build on them
3. **Consider the audience**: Users range from beginners to advanced Python developers

### Best Practices

1. **Start with the README**: Most UI/UX improvements should focus on making the README more accessible
2. **Maintain consistency**: Keep the style consistent with existing documentation
3. **Test examples**: Ensure any code examples you add actually work
4. **Consider all platforms**: The library works on macOS, Linux, and Windows

## Configuring Skills in VS Code

You can configure how Copilot Skills work in your VS Code settings:

1. Open Settings (`Cmd+,` or `Ctrl+,`)
2. Search for "GitHub Copilot"
3. Adjust settings like:
   - `github.copilot.enable`: Enable/disable Copilot
   - `github.copilot.editor.enableAutoCompletions`: Control auto-completions

## Using Skills with Specific Files

When working on specific files, you can provide file context to the skill:

```
@workspace #file:README.md How can I improve the installation section?
```

This tells Copilot to focus specifically on the README.md file when providing suggestions.

## Advanced Usage

### Combining Skills

You can combine the UI/UX skill with other capabilities:

```
Can you analyze the user experience of the API and suggest code improvements?
How can I make both the documentation AND the code examples more accessible?
```

### Iterative Improvements

Work iteratively with the skill:

1. Ask for an analysis: "What are the main UX issues in the README?"
2. Get suggestions: "How can I fix these issues?"
3. Implement changes: "Can you help me rewrite this section?"
4. Review: "Is this better for users?"

## Troubleshooting

### Skill Not Working

If the skill doesn't seem to work:

1. **Check your subscription**: Ensure GitHub Copilot is active
2. **Restart VS Code**: Sometimes a restart helps
3. **Check extensions**: Make sure all required extensions are installed and updated
4. **Internet connection**: Copilot requires an internet connection

### Getting Better Results

To get better results from the skill:

1. **Be specific**: Instead of "improve this", say "make the installation instructions clearer for Windows users"
2. **Provide context**: Mention what you're trying to achieve
3. **Iterate**: Refine your prompts based on the responses

## Additional Resources

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [VS Code Copilot Extension](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot)
- [GitHub Copilot Chat](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot-chat)

## Contributing

If you find issues with this documentation or have suggestions for improvement, please open an issue or submit a pull request on the [numbers-parser repository](https://github.com/masaccio/numbers-parser).
