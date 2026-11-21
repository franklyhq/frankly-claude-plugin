# Frankly for Claude

This plugin helps you contact your U.S. representatives from Claude using your Frankly account. Claude can find who represents you, help you write a message, publish it under your real name on Frankly, and send it to their offices. Nothing is published, sent or saved until you approve the exact preview in the conversation.

## What's inside

- **Frankly connector** (`.mcp.json`): connects Claude to Frankly's hosted server at `https://agentic-api.frankly.app/mcp/claude` over HTTPS. No local program runs and nothing is installed on your computer.
- **`frankly` skill** (`skills/frankly/SKILL.md`): teaches Claude the approval workflow: check your profile and address, find your representatives, show one complete preview, and report each office's result accurately.

Works in Claude on the web, Claude Desktop, Claude mobile and Cowork. Claude Code can't sign in to Frankly yet.

## Connecting your account

The first time Claude uses a Frankly tool, it opens Frankly's sign-in page at `connect.frankly.app`. Sign in with your Frankly account and approve the permissions on Frankly's consent page. This plugin contains no passwords, API keys, client secrets or tokens, and it never asks you for them in chat.

## What it sends and where

The plugin talks only to Frankly's server above. Depending on what you ask and approve, Frankly:

- reads your Frankly profile, saved address and representatives
- looks up and validates an address you type (using Google Maps), and saves it only after you confirm
- publishes your approved message under your real name in Frankly's public app and guest feeds
- sends your approved message, with the contact details shown in the preview, to up to five federal offices

Your street address, phone number and email are never shown publicly. See the [Frankly privacy policy](https://www.frankly.app/privacy) and [terms of service](https://www.frankly.app/terms-of-service).

## Disconnecting

Disconnect Frankly in Claude's connector settings, or sign in at [connect.frankly.app](https://connect.frankly.app/) and open **Manage connections**. Published posts stay up until you delete them in Frankly.

## Support

Frankly Support: [developers@frankly.app](mailto:developers@frankly.app). Full guide: [agentic-api.frankly.app/claude.md](https://agentic-api.frankly.app/claude.md).
