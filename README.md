# why-is-the-agent-slow-
The video outlines several strategies to address high latency in **AI agent systems**, particularly those used for tasks like **performance reviews**:

*   **Transitioning from Synchronous to Asynchronous Tools**: By shifting from synchronous execution—where tools wait for each other—to asynchronous calls, multiple independent tasks can run in parallel, drastically reducing wait times.
*   **Optimizing MCP Servers**: When utilizing *Model Context Protocol* servers, developers should filter for only the necessary tools. This practice limits unnecessary overhead and prevents **context bloat**, which helps the agent process information more efficiently.
*   **Strategic Caching and Context Injection**: For tools that handle stable data (such as employee records), performance can be improved by **caching** results or injecting them directly into the system prompt. This avoids the latency associated with redundant API calls.
*   **Tool Composition**: If specific tools have overlapping functions or are consistently used sequentially, they can be **merged or composed** into a single, unified tool to streamline the workflow.
*   **Avoiding Unnecessary Complexity**: While patterns like **batching** are effective in general software engineering, the speaker advises against adding the overhead of a **multi-agent architecture** if a single-agent system with optimized tools is sufficient for the task.
