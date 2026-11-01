# QuizLink MCP Server

**Track your learning journey, everywhere.** In line for coffee, waiting at the airport or between sets at the gym, QuizLink turns dead time into valuable skills.

QuizLink is a hosted (remote) MCP server. Connect it to ChatGPT, Claude or any MCP client and ask it to quiz you on any topic, or paste in your notes:

- Quizzes in the format you choose: multiple choice, fill-in-the-blank, match pairs, ranking or crosswords
- Flashcards from a topic or from your own notes
- Study courses with sections and units for a test, exam or interview
- Diagrams that explain a concept visually
- Short study-break games: chess, snake and a memory match

## Connect

| | |
|---|---|
| Server URL | `https://mcp.quizlink.net/stream` |
| Transport | Streamable HTTP |
| Auth | OAuth 2.0 with dynamic client registration (tools can be tried without signing in) |
| MCP Registry | [`net.quizlink/quizlink`](https://registry.modelcontextprotocol.io/v0.1/servers?search=net.quizlink) |

**Claude:** Settings → Connectors → Add custom connector → paste the server URL.
**ChatGPT:** Settings → Apps & Connectors → Developer mode → Create → paste the server URL.
**Other clients (Cursor, VS Code, Windsurf, Cline, Goose):**

```json
{
  "mcpServers": {
    "quizlink": { "type": "streamable-http", "url": "https://mcp.quizlink.net/stream" }
  }
}
```

## Example prompts

- "Quiz me on the causes of World War I."
- "Turn these notes into flashcards: ..."
- "Help me study photosynthesis for my biology test."
- "Show my QuizLink courses."

## Links

- Website: https://quizlink.net
- Docs: https://quizlink.net/mcp.html
- Privacy policy: https://quizlink.net/privacy.html
- Terms: https://quizlink.net/terms.html
- Support: support@quizlink.net

This repository holds the listing metadata for the hosted QuizLink MCP server. The server itself is operated by QuizLink.
