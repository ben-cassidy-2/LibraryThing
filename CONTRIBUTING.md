# Contributing to LibraryThing

Contributions are welcome in the form of **issues** and **pull requests**.

You can [submit an issue](https://github.com/ben-cassidy-2/LibraryThing/issues/new) to report a bug, request a new feature, suggest a performance improvement, or request better documentation or support on a particular issue.

To contribute code, you need to [fork this repository](https://github.com/ben-cassidy-2/LibraryThing/fork), create a feature branch on your fork, then open a pull request using the 'Contribute' button in your fork's homepage.

## Pull Request Format

Pull request titles should follow the [conventional commit](https://www.conventionalcommits.org/) specification. In this repository, PR titles should begin with one of:

| Prefix    | Used for                                                      |
|-----------|---------------------------------------------------------------|
| Feat:     | A new feature                                                 |
| Fix:      | A bug fix                                                     |
| Docs:     | Documentation only changes                                    |
| Style:    | Changes that do not affect the meaning of the code            |
| Refactor: | A code change that neither fixes a bug nor adds a feature     |
| Perf:     | A code change that improves performance                       |
| Test:     | Adding missing tests or correcting existing tests             |
| Build:    | Changes that affect the build system or external dependencies |
| CI:       | Changes to our CI configuration files and scripts             |
| Chore:    | Other changes that don't modify src or test files             |
| Revert:   | Reverts a previous commit                                     |


## Code Standards

### Style

In general, the style that the [.NET project uses](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions) applies.

### Memory Safety

Whilst C# is a beautifully safe language on the surface, this library is heavily dependent on manual pointer arithmetic. Any changes to `unsafe` blocks of code should be analysed and tested with extra rigour.

## Use of Generative AI

As a rule, **do not** commit a line of code that wasn't, at the very least, typed (and understood) by a human. Use of AI agents, as well as directly copy-pasting code from an AI chatbot, is not allowed due to the abundance of `unsafe` code.

It is permissible to consult AI assistants, including Copilot, or to have them check your solution or code. However, you should take care to double-check all AI-generated solutions, and ensure you *retype* its output rather than simply pasting it in. This is a self-policed policy to encourage understanding each line of code before you commit.

**If you have Copilot (or another AI assistant) enabled in your IDE, please:**
- Disable inline suggestions.
- Ensure all chats are in 'Ask' mode, to prevent the LLM making direct changes.
