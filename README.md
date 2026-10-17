# Quorum MCP

<img src="assets/quorum-icon.png" alt="Quorum AI" width="96" />

**AI’s second opinion.**

Quorum uses configurable Modes to gather and synthesize responses from AI models. Depending on the selected Mode, a deliberation can include multiple models, critique, judging, and synthesis. Results can help users examine different perspectives, including areas of agreement and disagreement.

Use Quorum inside your AI assistant to explore assumptions, compare architecture choices, evaluate implementation plans, and consider build-versus-buy decisions. Outputs are AI-generated and may be incomplete or incorrect.

## What the connector offers

- List the Quorum Modes available to your account.
- Request an estimate before running a deliberation.
- Run a selected Mode to compare AI perspectives.
- Retrieve a receipt with participating models, cost, scores, and latency where available.
- Create, validate, test, certify, and publish Modes, subject to your account permissions.

## Connect with Cursor

A Quorum account is required. Install the plugin and complete Quorum’s OAuth sign-in when Cursor prompts you. The plugin connects to `https://www.quorum.dog/mcp` using remote HTTP. No local server, package installation, or pasted API key is needed for this OAuth setup.

For a direct connection before marketplace approval, add this configuration to your Cursor MCP settings (`.cursor/mcp.json` for a project, or your global Cursor MCP configuration):

```json
{
  "mcpServers": {
    "quorum": {
      "url": "https://www.quorum.dog/mcp"
    }
  }
}
```

Enable Quorum in Cursor’s MCP settings and complete sign-in. Ask Cursor to list your Modes to check the connection.

## Connect with VS Code

Add the following to `.vscode/mcp.json` in your project. Enable the server and complete Quorum’s OAuth sign-in when prompted.

```json
{
  "servers": {
    "quorum": {
      "type": "http",
      "url": "https://www.quorum.dog/mcp"
    }
  }
}
```

You can also use the **MCP: Add Server** command and select HTTP, then enter the endpoint above.

## Connect with Claude or ChatGPT

Where your client supports custom remote MCP connectors, use `https://www.quorum.dog/mcp` and complete OAuth sign-in. Availability and setup depend on the client and account plan. See the [Quorum MCP guide](https://www.quorumllm.com/docs/guides/mcp) for client-specific instructions.

## Try it

1. “List the Quorum Modes available to me. Don’t run a deliberation.”
2. “Estimate a Quorum review of whether our five-person consultancy should build or buy its client onboarding system. Don’t run the panel yet.”
3. After reviewing the estimate: “Run that Quorum deliberation using the selected Mode.”
4. “Pull the receipt for that run. Show participating models, cost, judge scores, and latency where available.”

Other useful questions:

- “Get a Quorum estimate for comparing a modular monolith with microservices for this project. Don’t run yet.”
- “Use Quorum to review this implementation plan after I approve the estimate. Identify assumptions and tradeoffs.”

Estimates can return unavailable pricing fields; an unavailable price is not a zero-cost quote. Deliberations and other execution tools may incur usage charges. Follow the tools’ approval requirements and the user’s spending instructions. Report missing receipt fields as unavailable.

## Data and permissions

Prompts and context sent to Quorum are processed by the Quorum service and the model providers used for the selected Mode. Send only the context needed for the requested review. The connector also exposes tools that can save or publish Modes; use those only when requested and permitted by the connected account.

- [Website](https://www.quorumllm.com)
- [MCP documentation](https://www.quorumllm.com/docs/guides/mcp)
- [Support](https://www.quorumllm.com/help)
- [Privacy policy](https://www.quorumllm.com/privacy.html)
- [Terms](https://www.quorumllm.com/terms.html)

This repository contains public connector configuration, setup documentation, and brand assets. Quorum’s hosted application runs separately.
