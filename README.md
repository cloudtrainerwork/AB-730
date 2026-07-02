Here is a detailed breakdown of each concept tested on the AB-730 exam, drawing directly from the verified study guides and exam experiences:

### 1. Understand Generative AI Fundamentals (25–30%)

**Copilot Capabilities in Apps**
The exam tests your understanding of what Copilot *can* and *cannot* do within specific apps:
*   **Word:** It can draft documents, summarize content, and format text, but it cannot change document metadata or properties like margins or page orientation.
*   **Excel:** It can analyze data, generate formulas, and create visualizations or charts from natural language. However, it cannot write VBA code, automatically connect to external databases, or create complex pivot tables.
*   **PowerPoint:** It can take a lengthy Word document and automatically convert it into a structured presentation with slides, layouts, and speaker notes. It cannot build advanced, complex animations.
*   **Outlook:** It can draft emails and summarize long, back-and-forth email threads. It cannot schedule emails to be sent at a later time.
*   **Teams:** It can summarize meetings and highlight key decisions, but only if the meeting was recorded and transcribed. 

**Chat vs. Agents**
You must know the difference between general chat and purpose-built agents. **M365 Copilot Chat** is a broad conversational interface that can toggle between "Work Mode" (searching organizational data) and "Web Mode" (searching the public internet). **Agents** are highly specific, custom-built assistants designed to execute a single workflow or answer targeted questions (e.g., an HR policy agent).

**Context and Grounding**
This focuses on the flow of data and **Retrieval-Augmented Generation (RAG)**. When you send a prompt, it goes to **Microsoft Graph** for "pre-processing" or "grounding," which pulls your relevant files and emails to give the AI context. It is then sent to the Large Language Model (LLM) to generate text, and finally goes back to Graph for "post-processing" to verify the answer before returning it to you. RAG is what ensures your answers are based on your real workplace data rather than generic internet training data.

**Responsible AI**
You must memorize Microsoft's six responsible AI principles: **Fairness, Reliability & Safety, Privacy & Security, Inclusiveness, Transparency, and Accountability**. 
*   **Risks:** You will be tested on identifying **hallucinations** (when the AI confidently fabricates incorrect information) and **prompt injection** (when malicious actors hide instructions in documents to trick the AI into unauthorized actions). 
*   **Human-in-the-loop:** The exam stresses that AI is for drafting and summarizing; definitive legal, financial, or compliance decisions always require human accountability and review.

**Data Security and Governance**
A foundational rule for the exam is that **Copilot strictly respects existing M365 permissions**. It will never surface a file that the logged-in user does not already have access to. Furthermore, your prompts and organizational data are encrypted in transit and are **never stored or used to train the public LLM**. The exam heavily tests **Microsoft Purview** as the backbone for enforcing data governance, compliance policies, and sensitivity labels. 

### 2. Manage Prompts and Conversations by using AI (35–40%)

**Prompt Engineering**
Effective prompts must contain four specific elements: **Goal, Context, Source, and Expectations (like tone or format)**. You are also tested on how to refer to sources directly in your prompt: using **/** (slash) to reference files, **#** (hashtag) to reference meetings or topics, and **@** (at symbol) to reference people or other agents. 

**Conversation Management**
The exam goes into the specific user interface steps for managing your chats. You need to know how to save, share, and schedule prompts within the platform so your entire department can reuse them. You also need to know that users can manually delete their chats, but doing so does not override Microsoft's backend **default 90-day retention policy**. 

**Creating and Managing Agents**
You will be tested on the difference between building an agent in **Copilot Studio** (for connecting to APIs and deeper integrations) versus the built-in M365 agent builder. When configuring an agent, you must know its components: a name, description, persistent instructions, up to **20 knowledge sources** (files, folders, or SharePoint sites), and up to **8 suggested prompts**. You also need to know that while agents can be shared with team members, modification permissions are tightly controlled via role-based access. 

### 3. Draft and Analyze Business Content by using AI (25–30%)

**Document Drafting**
You must know the exact workflows for content creation. For example, in Outlook, the correct workflow is to first use Copilot to summarize a 35-message thread to gain context, and *then* use Copilot to draft an informed reply. You also need to understand how Copilot can move data between apps, such as turning a Word document into a PowerPoint presentation.

**Specialized Agents: Researcher vs. Analyst**
The exam heavily tests your ability to distinguish between these two pre-built agents:
*   **Copilot Researcher:** Used for deep, multi-source information gathering, strategy planning, and synthesizing knowledge from the web and documents to create reports.
*   **Copilot Analyst:** Used strictly for structured data. It processes Excel or CSV files to generate charts, identify numeric trends, recognize patterns, and utilizes a code interpreter (Python) for complex calculations.

**Collaboration Tools: Copilot Pages vs. Notebooks**
*   **Copilot Pages:** Built on Microsoft Loop. They are lightweight, **real-time collaborative** workspaces where you can turn a chat response into an editable page alongside your team.
*   **Copilot Notebooks:** Designed for structured, multi-step, **asynchronous** projects. Notebooks allow for iterative prompting (refining ideas step-by-step) and can generate audio overviews, but they do *not* have long-term chat memory across different sessions. 

**Meeting Management**
For Copilot to work in Teams, the meeting must be recorded and transcribed. A major limitation tested on the exam is that Copilot in Teams often requires manual activation before the meeting begins; it does not automatically jump into every meeting to record and summarize.

**Memory and Instructions**
You must understand how Copilot stores context:
*   **Custom Instructions (Memory):** Users can set persistent preferences (e.g., "always respond in bullet points under 200 words"), which Copilot automatically applies to all future chats.
*   **Temporary Chats:** Functions like an "incognito mode." It allows you to have a conversation that ignores your persistent memory settings, and the chat is not saved in your history. 
*   **Siloed Context:** Copilot does *not* behave like ChatGPT with a universal long-term memory. It does not carry context from one chat session to another, nor does it share memory between different agents.
