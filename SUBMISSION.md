# Cursor submission checklist

## Listing

- Name: Quorum AI
- Plugin identifier: quorum
- Tagline: AI’s second opinion
- Description: Compare AI perspectives on a question with configurable Quorum Modes.
- Website: https://www.quorumllm.com
- Category suggestion: Productivity / Developer Tools (choose the closest available category)
- Endpoint: https://www.quorum.dog/mcp
- Authentication: OAuth
- Privacy: https://www.quorumllm.com/privacy.html
- Support: https://www.quorumllm.com/help

## Publish preparation

1. Public repository: https://github.com/quorum-dog/quorum-mcp. The plugin manifest is `.cursor-plugin/plugin.json`.
2. Confirm the committed README, logo, manifest, and MCP configuration are visible publicly.
3. Test installation and OAuth in Cursor. List Modes, request an estimate without running, then explicitly authorize a deliberation and retrieve its receipt. Check that estimate-only requests do not execute a panel.
4. Submit the public repository URL at https://cursor.com/marketplace/publish.

## Validation status

Package structure, JSON syntax, manifest paths, logo inclusion, and endpoint configuration were checked during preparation. The endpoint and account workflow were exercised through the connected Quorum MCP earlier in this session. A Cursor-specific installation and OAuth test has not been performed. This package has not been submitted to Cursor.

Reference: https://cursor.com/docs/reference/plugins
