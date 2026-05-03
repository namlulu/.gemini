# Gemini CLI Workspace

This directory contains the configuration, state, and history for Gemini CLI.

## Directory Structure

- `agents/`: Custom agent definitions and configurations.
- `history/`: Session history and logs for past interactions.
- `tmp/`: Temporary files and working directories for active sessions.
- `google_accounts.json`: (Sensitive) Google account information.
- `oauth_creds.json`: (Sensitive) OAuth2 credentials.
- `settings.json`: User-specific settings and preferences.
- `state.json`: Global state information for the CLI.

## Security Note

This folder contains sensitive information including OAuth tokens and account details. **Never share the contents of `.json` files (except `settings.json` and `projects.json`) or commit them to a public repository.**
