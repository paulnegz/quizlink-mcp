# Installing the QuizLink MCP server

QuizLink is a hosted, remote MCP server. Nothing needs to be installed or built.

1. Add this entry to the MCP settings file:

```json
{
  "mcpServers": {
    "quizlink": {
      "type": "streamableHttp",
      "url": "https://mcp.quizlink.net/stream"
    }
  }
}
```

2. Restart or reload MCP servers. The tools (create_quiz, create_mcq, create_flashcards, study_concept, my_courses and others) become available.
3. Tools work without signing in for a few free uses. To save courses and progress, the client will open QuizLink's OAuth sign-in page when needed.

Test prompt: "Quiz me on the solar system."
