# Personal App

Personal App is an AI-powered Android workspace that evolves through natural-language commands.

## Concept

Start with a clean, infinite canvas and an AI message bar. Connect an AI provider with an API key, then ask Personal AI to build and modify your workspace.

Examples:

- "Create a todo list."
- "Create a digital clock."
- "Make a Pomodoro timer."
- "Create a notes section."
- "Remind me every day at 8 PM to study."
- "Move the clock to the top right."
- "Make the todo widget larger."
- "Undo what you just did."

## Core architecture

The AI does not execute arbitrary code or directly modify Android source code.

Instead:

User → AI Chat → AI Model → Structured Tool Calls → Tool Validator → Capability API → Personal App Engine

The Capability API is responsible for controlled operations such as:

- createWidget
- updateWidget
- deleteWidget
- moveWidget
- resizeWidget
- createPage
- createNotification
- saveData
- readData
- changeStyle
- undoAction
- redoAction

## Planned features

- Infinite canvas with pan and zoom
- AI-controlled widgets
- Todo, Notes, Clock, Timer, Counter, Button, Text and Progress widgets
- Scheduled Android notifications
- Persistent local data
- Undo / Redo and action history
- Multiple pages
- Gemini API integration
- Provider abstraction for future AI models
- Secure API-key storage
- Offline access to the local workspace

## Design

The UI should be modern, minimal and professional, with calm colors, clean typography, rounded components, subtle shadows and generous whitespace.

Avoid neon, cyberpunk, excessive gradients, gamer aesthetics and cluttered dashboards.

## Security

AI-generated operations are treated as untrusted input and must be validated before execution.

The AI must not automatically access contacts, SMS, camera, microphone, files, other applications or location.

## Status

🚧 Project initialization — Android implementation to follow.

## License

License will be selected when the project reaches its initial implementation stage.
