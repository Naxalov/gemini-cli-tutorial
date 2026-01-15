# Getting Started with Gemini CLI

This document will guide you through the initial steps of using the Gemini Command Line Interface.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Obtaining an API Key](#obtaining-an-api-key)
- [Configuration](#configuration)
- [Your First Command](#your-first-command)
- [Checking the Command History](#checking-the-command-history)
- [Next Steps](#next-steps)

## Prerequisites

Before you begin, ensure you have:
- The Gemini CLI installed (refer to the main `README.md` for installation instructions).

## Obtaining an API Key

To use the Gemini CLI, you need an API key. Here's how to get one:
1. Go to the Gemini API website.
2. Sign in with your Google account.
3. Create a new project and generate an API key.

## Configuration

Once you have your API key, you need to configure the Gemini CLI to use it.
```bash
gemini config set api_key YOUR_API_KEY
```

## Your First Command

Now you're ready to run your first command. Try a simple prompt:
```bash
gemini "hello world"
```
Or using the prompt flag:
```bash
gemini --prompt "hello world"
```

## Checking the Command History

You can view your command history by running:
```bash
gemini history
```

## Next Steps

You are now ready to explore more advanced features of the Gemini CLI.