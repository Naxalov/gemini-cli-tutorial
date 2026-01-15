# Gemini CLI Tutorial

This repository will contain tutorials and examples for using the Gemini Command Line Interface.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Basic Commands](#basic-commands)
- [Slash Commands](#slash-commands)
- [Advanced Usage](#advanced-usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

### MacOS (using Homebrew)

To install the Gemini CLI on macOS using Homebrew, follow these steps:

1.  **Open your terminal.**

3.  **Add the Gemini tap:**
    ```bash
    brew tap gemini/gemini-cli
    ```
4.  **Install the Gemini CLI:**
    ```bash
    brew install gemini-cli
    ```
5.  **Verify the installation:**
    ```bash
    gemini --version
    ```
    This command should display the installed version of the Gemini CLI.

## Getting Started

For a detailed guide on how to get started with the Gemini CLI, please refer to the [Getting Started guide](getting-started.md).

## Command Types

The Gemini CLI has two types of commands:

1.  **CLI Arguments:** These are flags and options you pass when starting the `gemini` executable (e.g., `--help`, `--version`, `config`). They control the initial setup, configuration, and mode of the CLI.
2.  **Slash Commands:** These are commands used *within* an interactive session (e.g., `/help`, `/clear`). They help you manage the current conversation and session state.

## Basic Commands

Here are some of the most common commands to get you started with the Gemini CLI.

### General

-   `gemini --help`: Show the help message, which includes a list of all available commands.
-   `gemini --version`: Display the installed version of the Gemini CLI.

### Configuration

-   `gemini config list`: List all your current configuration settings.
-   `gemini config get <KEY>`: Retrieve the value of a specific configuration key.
    -   Example: `gemini config get api_key`
-   `gemini config set <KEY> <VALUE>`: Set a new value for a configuration key.
    -   Example: `gemini config set api_key YOUR_API_KEY`

### History

-   `gemini history`: View a list of your recent commands.

### Interaction

-   `gemini "<PROMPT>"`: The most fundamental command. It sends your text prompt to the Gemini model and returns the response.
    -   Example: `gemini "What is the speed of light?"`
-   `gemini -p, --prompt <text>`: Send a text prompt using a flag.
    -   Example: `gemini --prompt "What is the speed of light?"`

## Slash Commands

When you are in an interactive session, you can use the following slash commands:

- `/help`: Show available slash commands.
- `/bug`: Report a bug or provide feedback.
- `/clear`: Clear the current session history.
- `/exit`: Exit the interactive session.

## Advanced Usage

### Custom Commands

You can define custom commands to streamline your workflow.

- `gemini custom list`: List all your defined custom commands.
- `gemini custom add <NAME> <PROMPT>`: Create a shortcut for a frequently used prompt.
    - Example: `gemini custom add translate "Translate the following text to French: "`
- `gemini <NAME> <TEXT>`: Execute a custom command.
    - Example: `gemini translate "Hello, how are you?"`

## Contributing

How to contribute to this project.

## License

The license for this project.
