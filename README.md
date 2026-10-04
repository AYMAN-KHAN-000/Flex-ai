# FLEX Chat

FLEX Chat is a lightweight, single-page AI chat interface. It runs in the browser without a build step or application server.

## Features

- Streamed assistant responses from the configured AI service
- API key entry through the in-app **Access key** dialog
- Recent conversations available in the sidebar and mobile drawer
- Collapsible desktop sidebar and responsive mobile layout
- Dark blue theme with animated gradient frame and matching scrollbars
- Creator links to [GitHub](https://github.com/ayman-khan-000) and [Portfolio](https://protfoolio.vercel.app)

## Getting Started

1. Open `index.html` in a modern web browser. No package installation or build command is required.
2. Select **Access key**, enter a valid API key for the configured service, and select **Save key**.
3. Type a message and submit it to start a conversation.

Without a key, FLEX displays an access-denied response when a message is submitted.

## Configuration and Data

- The chat model is selected in `index.html`; there is no model picker in the interface.
- The API key is held in browser memory for the current page session. It is not saved and is cleared when the page is reloaded or closed.
- Conversation history is also held in memory and is cleared when the page is reloaded or closed.
- The page sends requests directly from the browser to the configured AI service. No application server or server-side key protection is included.

## Security

Because requests are made directly from the browser, an API key entered into FLEX is available to that browser and is sent with requests to the configured service. Do not put a personal key in the source code or publish this static page for unrestricted public use with a shared key. For a public deployment, route requests through a backend that authenticates users and protects the service key.

## Project Files

- `index.html` - application markup, styles, and client-side logic
- `icon.webp` - FLEX logo used in the page
