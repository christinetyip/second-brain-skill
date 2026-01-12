# Second Brain

A Clawdbot skill for personal knowledge management powered by [Ensue](https://ensue-network.ai).

## What it does

Captures and retrieves your understanding over time. Not a note dump - a structured system for knowledge that compounds.

- **Concepts** - How things work, with diagrams and mental models
- **Toolbox** - Tools you've actually used, with your experience
- **Patterns** - Reusable solutions to common problems
- **References** - Quick-lookup cheatsheets and syntax

## Installation

1. Get an Ensue API key at https://www.ensue-network.ai/dashboard

2. Add to your Clawdbot config (`~/.clawdbot/clawdbot.json`):
```json
{
  "skills": {
    "entries": {
      "second-brain": {
        "apiKey": "your-ensue-api-key"
      }
    }
  }
}
```

3. Copy the `second-brain` folder to your Clawdbot workspace skills directory

4. Restart the daemon: `clawdbot daemon restart`

## Usage

Talk to Clawdbot naturally:

- "Save this concept about caching"
- "What do I know about databases?"
- "Add Docker to my toolbox"
- "Show my toolbox"
- "Search for authentication patterns"

## Structure

```
public/
  concepts/[domain]/[name]     How things work
  toolbox/[category]/[name]    Tools you use
  patterns/[domain]/[name]     Reusable solutions
  references/[topic]/[name]    Quick-reference material

private/
  notes/                       Scratchpad
  journal/                     Dated reflections
```

## License

MIT
