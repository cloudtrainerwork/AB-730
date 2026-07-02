In addition to the core concepts already discussed, recent exam takers and study guides highlight several other heavily tested areas and specific "gotchas" on the AB-730 exam:

**The "Limitations Mindset"**
A major theme of the exam is testing your knowledge of what Copilot **cannot** do, rather than just what it can do. You must be able to identify its strict boundaries:
*   Copilot cannot access local files stored on your computer's hard drive; files must be stored in the cloud (like OneDrive or SharePoint).
*   It cannot bypass security, escalate access, or invent data when it faces a permission block. 
*   It cannot make definitive legal, financial, or compliance decisions; human review and accountability are strictly required.
*   Many wrong answers on the exam will sound technically impressive but violate these core Microsoft 365 Copilot limitations.

**Nitpicky UI Details and Workflows**
The exam goes surprisingly deep into the actual user interface and the precise order of operations. You will be tested on:
*   The exact tabs, button names, and steps required to build an agent, save a prompt, or schedule a prompt. 
*   The correct sequence of actions for specific tasks, such as first summarizing a long Outlook thread before using the draft feature to reply. 

**The Exact Flow of Data**
You will be tested on the precise journey a prompt takes when you interact with Copilot. You must know this sequence:
1.  **Pre-processing (Grounding):** Your prompt goes to **Microsoft Graph** to gather relevant organizational data and context.
2.  **LLM:** The grounded prompt is sent to the Large Language Model.
3.  **Post-processing:** The generated response goes *back* to Microsoft Graph to be verified against your data and checked for hallucinations before it is presented to you.

**Agent Governance and Modification Limits**
While creating and sharing agents is tested, the exam heavily emphasizes the governance boundaries around them. Specifically, you must know that while users can share an agent, **modifying** that agent is tightly controlled through role-based access and strict change management protocols. If an exam option assumes any user can edit an agent they have access to, it is incorrect.

**Data Boundaries and Specific Add-ons**
*   **Microsoft EU Data Boundary:** You must know this specific commitment, which ensures that European customer data is processed and stored entirely within the European Union to comply with GDPR and other regulations.
*   **Custom Agent Add-ons:** You should know that when building a custom agent, you can specifically enable two powerful add-ons: a **Python code interpreter** (for data analysis and charts) and an **image generator**.
*   **Work Mode vs. Web Mode:** In the M365 Copilot chat, you must know the difference between toggling "Work Mode" (which strictly prioritizes internal organizational data) and "Web Mode" (which searches outside the organization for information). 

**Exam Format Specifics**
Finally, you should be prepared for the structure of the exam itself. It consists of 40 to 60 questions that must be completed in 45 minutes. The question formats include standard multiple-choice, drag-and-drop, yes/no options, and hotspot questions. Notably, there are **no case studies** on the AB-730 exam.
