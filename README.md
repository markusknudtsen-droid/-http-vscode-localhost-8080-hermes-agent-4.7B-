# Hermes Agent 4.7B – VS Code Gateway

## Gateway URL

Use the following URL to connect to the Hermes Agent (4.7B) from VS Code:

```
http://localhost:8080
```

## Quick Start

1. Make sure the Hermes Agent server is running on your machine (default port **8080**).
2. Open VS Code.
3. Open the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`) and run **"Open URL"**, or simply click the link below in your browser / terminal:

   **[http://localhost:8080](http://localhost:8080)**

4. The workspace is pre-configured (see `.vscode/settings.json`) to point VS Code's language-model / Copilot gateway at this address.

## Configuration

The gateway endpoint is stored in `.vscode/settings.json`:

```json
{
  "hermes.gatewayUrl": "http://localhost:8080"
}
```

You can change the port by editing that file if your Hermes Agent runs on a different port.

## hermes-gateway.json

A machine-readable configuration file `hermes-gateway.json` is included at the root of this repository:

```json
{
  "name": "Hermes Agent 4.7B",
  "gatewayUrl": "http://localhost:8080",
  "version": "4.7B"
}
```