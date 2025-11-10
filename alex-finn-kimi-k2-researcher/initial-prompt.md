Build a Kimi K2 Thinking Demo App Create a web app that demonstrates the Kimi K2 Thinking model's extended reasoning and multi-tool capabilities. The app should:
Tech Stack: Next.js, TypeScript, Tailwind CSS v3, React
Features:
Accept research queries (e.g., "Compare Notion, Obsidian, and Roam Research")
Display real-time thinking/reasoning as it happens
Show all tool calls as they execute with arguments and results
Display metrics (thinking tokens, tool calls, elapsed time, input/output tokens)
Show final research report in markdown
Tools: The model should have access to:
web_search: Search the web for information (use Tavily API)
analyze_data: Execute Python code for data analysis and visualization
create_pdf_report: Generate professional PDF research reports
UI Layout:
Input area for research queries with 3 example prompts
Metrics panel showing real-time stats
Three-column layout showing: Thinking (left) | Tool Calls (middle) | Results (right)
Each panel scrolls independently with 600px fixed height
API: Use the Moonshot API (Kimi K2 Thinking model) with streaming responses
Example Queries:
"Research Notion, Obsidian, and Roam Research. Find pricing, create a comparison chart, and generate a PDF report."
"Analyze the top 3 AI coding assistants. Research pricing and features, create visualizations, and export a PDF."
"Research cloud storage providers. Find pricing tiers, calculate cost per GB, create a chart, and generate a PDF decision matrix."
Environment Variables:
MOONSHOT_API_KEY (from Moonshot AI)
TAVILY_API_KEY (from Tavily)