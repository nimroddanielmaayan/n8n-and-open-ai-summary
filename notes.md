# n8n and OpenAI PlatformSummary

## General

### General Information - Automations and n8n

- I am currently working on this tutorial: <https://youtu.be/u7ktVHkd8DI>, I
  already set up payments to OpenAI

- I want to create one "Nimrod Bot" workflow that will use WhatsApp, and one
  that will use a "public" web chat window, so that potential clients can
  interact with it themselves. This bot needs to include at least one "tool",
  like offering the user to send an email to me. More complex tool calls can be
  added later, like scheduling a meeting with me, etc

- Reminder - the assistant needs to be notified about the tools that it can run,
  (like send an email), and when it needs to run them, in its system
  instructions

- n8n recently added a "Data Table" node, which is like Google Sheets, but
  native

- The next thing that I have to do for "Nimrod Bot" is to write a PDF with
  questions and answers, to upload to the OpenAI Platform

- n8n might be a "gold rush" for a while. So it's something that can make a lof
  of money in the short term, but will become very common and "comoditized" in
  the long run

- Therefore, speed is of the essence

- My n8n platform URL: <https://mayandigital.app.n8n.cloud/>

- Workflow templates: <https://n8n.io/workflows>

- (check more WhatsApp "example workflows" - this is the most common client
  request. Maybe even create an entire "WhatsApp workflows" portfolio)

- Currently, it looks like there's no way to link to a "public portfolio" or to
  individual workflows. The only way to show the portfolio to potential clients
  is using screen share or video capture

- There are templates and tutorials for virtually every type of workflow and
  automation... So I can create an example for any kind of project that a
  potential client might want

- n8n is short for "nodemation", which basically means "automation using nodes"

- The way to get good business results is to solve a meaningful business problem
  in a good way, and then repeat the process in a wahy that's as automatic as
  possible. Eventually, it's possible to even develop a software (SASS) that can
  solve this problem

### My Progress - Types of Projects that I've Done

- WhatsApp\web chatbot
- RAG
- Google Calendar integration
- Google Mail integration
- Google Sheets integration
- Local n8n database integration
- Leads aggregation and qualification (to be completed)
- (more to come)

(I need to do projects that end up in impressive demos)

### My Progress - To Do

To do - tutorials\videos:

- Practice: Webhooks\Builfing an API server (and test using Postman), error flow
  (and implement in my portfolio), save to GitHub flow (it's in the existing
  templates)
- <https://docs.n8n.io/try-it-out/quickstart/>
- <https://docs.n8n.io/try-it-out/tutorial-first-workflow/>
- <https://www.youtube.com/watch?v=GVBjKEWHiF8>
- <https://www.youtube.com/watch?v=aB2h3SzCZwc>
- <https://www.youtube.com/watch?v=PT6payqqvuk>
- <https://www.youtube.com/watch?v=fWtXJswvUcA>
- <https://www.youtube.com/watch?v=pMIiZfqfbCo>

To do - flows to go over:

- <https://n8n.io/workflows/2465-building-your-first-whatsapp-chatbot/>
- <https://n8n.io/workflows/2845-complete-business-whatsapp-ai-powered-rag-chatbot-using-openai/>
- <https://n8n.io/workflows/6771-whatsapp-rag-chatbot-with-supabase-gemini-25-flash-and-openai-embeddings/>
- <https://n8n.io/workflows/2845-complete-business-whatsapp-ai-powered-rag-chatbot-using-openai/>
- <https://n8n.io/workflows/9043-whatsapp-support-bot-with-google-drive-rag-gpt-41-mini-and-cohere-reranking/>
- <https://n8n.io/workflows/4827-ai-powered-whatsapp-chatbot-for-text-voice-images-and-pdf-with-rag/>

## Official n8n Tutorials - Summary

### Official n8n Video Tutorials

- <https://www.youtube.com/playlist?list=PLlET0GsrLUL59YbxstZE71WszP3pVnZfI>

- <https://www.youtube.com/playlist?list=PLlET0GsrLUL5bxmx5c1H1Ms_OtOPYZIEG>

### Tutorial Subject 1 - Basics

- When there's an error, "copy to editor" becomes "debug in editor", and then we
  can retry. Using "edit output" for debugging is also a good technique

- At the end of a work day, it's recommended to save the workflows locally, or
  to use a GitHub automation

- Every input and output are built of a list of JSONs, also called "items"

- Not every flow failure will result in an error (for example - an empty reply).
  That's what the "throw error" node shoud be used for

- It's important to add contact details to an error flow, at least an email

- In the n8n community forum, it's possible to request help from the company's
  support

- It's always good practice to search for existing templates, before trying to
  build something from zero

- User types: Owner, admin, member

- Sharing credentials between projects can be done without exposing the actual
  credentials

- Then n8n API is used for several use cases, like managing workflows using
  external software

- The most common\useful nodes:

  - Chat Trigger
  - n8n Form Trigger
  - Manual Trigger
  - Schedule Trigger
  - Error Trigger
  - Filter
  - HTTP Request
  - Webhook
  - Respond to Webhook
  - Edit Fields
  - If
  - Switch
  - Loop
  - Execute Sub-Workflow
  - Call n8n Workflow Tool
  - n8n
  - Code
  - Split Out
  - Aggregate
  - Merge
  - Summarize
  - Stop and Error
  - Wait
  - Data Table
  - Execution Data
  - No Operation

- Actions\Apps: Allow us to interact with 3rd party applications

- Mapping: The first step to any good automation! Mapping can be done with any
  graphic software, or even on paper. There's no need to plan which nodes to use
  at this point, just the general logical flow of the process. Maping

  1. Fully understanding the task
  2. Tools that will be used
  3. Feasibility\reliability of the automation
  4. Estimation of the workload the automation will handle
  5. Points of human intervention (sometimes)

### Tutorial Subject 2 - Advanced Concepts

- It's common practice to write JSON names with lowercase letters and an
  underscore, like: first_name, last_name, etc

- Nodes are activated from top to bottom, and then from left to right. There
  must always be a logical order to when things happen

- It's possible to take an output from one node to several node branches. In
  this case, the output is copied in full

- Sometimes a node should only be executed once - in which case, it has to be
  marked to execute once

- The merge node is the only one that requires 2 inputs. It can
  combine\append\choose. There are several possible ways to match data, like in
  SQL

- The loop node is useful if there's an API limitation, or any other data size
  limitation

- The node's "output runs": Here, it's possible to scroll through the outputs of
  the different items

### Tutorial Subject 3 - Code and APIs

- In the n8n docs, there's a list of all the built-in functionalities that can
  be used in nodes. These functionalities are indicated by a $ sign

- The Code Node: It's important to remember that it must always retern either a
  list of JSONs or a single JSON. At the minimum, it must return empty data. The
  Code Node can actually replace many of the other nodes, but it's best practice
  to use thr more basic nodes when possible, for clarity and simplicity

- Webhook Node: Webhooks are like a "doorbell" that indicates that a "package
  has arrived". It can also be thought of as an "API server" node

- HTTP Request Node: This node is like "Postman in a node". It allows the flow
  to call a REST API. IT has several built-in options like pagination (multiple
  requests), authentication, etc

- We can import a curl command into an HTTP Request Node. curl is a command line
  tool for making HTTP requests manually. Many times, an APIs documentation will
  provide the curl version of commands, and that can save us time

- In a code node, it's possible to do a console.log and then to use the browser
  console to see the output

### Tutorial Subject 4 - Best Practices

- It's recommended to use pinning as much as possible, in order to save time.
  Oinning should be done at the stage at which we already finished working on,
  and so the pin should "advance" along the workflow with time

- Once pinning is used, the flow can be cativated step-by-step or all at once,
  using the pinned data

- Edit output: Is useful for edge cases, such as taking data and changing a
  specific value to "null", in order to simulate such a case

- Data can be copied from one execution to another. This can be useful if an
  execution failed and we want to debug it

- We can use mockaroo.com to create mock JSON data

- Another good practice is to create a Manual Trigger Node with mock data. It
  can be deleted once the flow is done

- Sub Workflows: This is how we can do modulization and reusability. Every Sub
  Workflow starts with an Execute Workflow node and should end with a No
  Operation node. And then, its final data is transfered to the next node after
  it (in the parent workflow)

- It's good practice to end every workflow with a No Operation node, and to call
  it "End of flow"

- Sticky notes can be used to document a workflow

- The idea of a "workflow owner": This refers not to authority, but to tagging
  the person who is responsible for the workflow (either on of our team members
  or one of the client's team members)

- In order to "inject" a non-changing JSON with non-changing data, it's possible
  to use the Code node with this command:

```javascript
return [
  {
    // JSON data...
  }
];
```

This node will always return the same JSON data, no matter what its input is. On
the other hand, this node does "care" when it's being activated and where it's
sending its output to, and so it does need to have both an input node and an
output node

- It's recommended when working with an external API, to always check if the
  status code is not 200, and to use an Error node if that's true

### Tutorial Subject 5 - Errors and Error Handling

- It's good practice to "categorize" errors, like 500 errors (server errors,
  usually not our fault), 400 errors (client errors, usually our fault), etc.
  This is done using code. It's also good practice to manage different error
  types differently, like sending them to the appropriate prople

- It's possible to create an "advanced error workflow", to use the n8n node in
  order to reciever the tag of whoever's responsible for the workflow that's
  erroring, and and in that way "standardize" the error handling process

### Tutorial Subject 6 - Working with Files

- When working with files, we'll have the "binary" option available in the
  output section of the node, alongside JSON\schema\table. From there, we can
  preview or download the file

- n8n has specific nodes for working with files, like the Zip\Unzip nodes

- Several files that are returned form a node can be considered as one item. In
  this case, it's possible to use a Code node to split these into separate
  output items

### Tutorial Subject 7 - Enterprise Features

- The enterprise plan allows us to create a custom log of the executions data.
  This data can be collected using the Execution Data node. This can also be a
  good way of sharing the execution data with the client, without having to give
  access the editor dashboard

- Git versioning is only available in the enterprise plan. But, saving to git is
  possible either manually or using a workflow

- Variables: Allow managing data in a more efficient way

- External Secrets: For using with external key-keeping services

- SSO\LDAP\Log Streaming: More relevant for large businesses\agencies

## n8n - Other Topics

### Retainer Clients

- All n8n clients need to have at least a minimal "retainer" contract, since
  they need to use a server that needs to be paid for, maintained and updated
  periodically

### Keeping Things Organized

- In order to keep things organized, it might be a good idea to name projects
  like this: "Client Name: Project Name"

- Internal projects (like my portfolio) should have a client name of "Internal"

- The "define using AI" option is useful, when the information that needs to be
  passed between nodes is dynamic and not known in advance

### n8n Tool Calling

- Code tools - these can be used, for example, to remove annotations from a PDF
  response, and so on

### Assistants

- Remember - assistants need to be notified about the tools that they can run,
  and when they need to run them. This is done in the assistant's system
  instructions

### Testing

- Always test before shipping to production!

- n8n has nice testing tools

## Chatbots\WhatsApp Chatbots

### General Information - WhatsApp Chatbots

- "WhatsApp Business Coexistence" - A way supported by Meta to combine a
  business WhatsApp number with an API. It's currently in beta mode, and
  available only in a few countries (including the US). Might be relevant for
  Upwork clients

- The "Evolution API" is a pirated way of bypassing Meta and combining a
  business WhatsApp account with an API. Could lead to the number being blocked.
  Don't use for clients

- For now, the best way to use WhatsApp is with Twilio, and to rent a new number

- An Israeli WA number on Twilio costs about $15 a month, and usage costs about
  $5 for every 1,000 messages sent

- Meta allows the API to "initiate" messages only in very specific templates
  (marketing, utility, authentication). Sending "freeform" messages is only
  possible if the user sent us a message first (and then we have a 24-hour
  window to send an API response). Meta are doing this in order to prevent
  WhatsApp from becoming a spam app, and that makes sense

- I prefer to create a Twilio account for every client. In the future, maybe I
  will use Twilio's "agency" account feature. I have to apply for it in their
  dashboard

- In addition, the client will have to pay for OpenAI API credits

- ManyChat is a simple, no-code platform for combining messages from WhatsApp
  and all the other social networks into a single dashboard, using basic
  automation for pre-written lead qualification questions, and so on

### The Twilio Platform

- ...

## n8n Self Hosting (on Hostinger)

### License - n8n Self Hosting

- The n8n free self hosting license allows for "personal, hobby, or internal
  non-commercial" use only. Commercial use is only allowed with a commercial
  license

- In any case, at some point I'll want to do an advanced paid plan, for the
  premium features

- If a client wants to manage his own n8n account for his own internal uses, I
  recommend self hosting. If it's for providing services to his clients, I
  recommend using the n8n cloud, either independently or as part of my n8n cloud

- <https://n8n.io/pricing>

## The OpenAI Platform - Chatbots, Assistants, Agents, Agent Builder, Agent Kit and More

- "Assistants" are like "augmented chats", that have been modified with custom
  instructions, data, tools and so on

- Note: External APIs, like the OpenAI API, "think" of n8n like any other web
  app that's connected to them

## Prompt Engineering and the OpenAI Cookbook

### Prompt Engineering Basics

- I saved in this project, undert the "info" folder, a few resources for prompt
  engineering, including a markdown guide

- {{variable}} can be used to define variables in a prompt. The variables also
  need to be defined in the

- Practical prompt engineering tips from Nick Saraev:
  - Keep prompts as short as possible
  - Use the "playground" interfaces, not the "commercial" (public) interfaces.
    This is true for all AI models, not just OpenAI\ChatGPT
  - The "commercial" interfaces include system prompts that are aimed at
    convincing users to get a premium license. This isn't always aligned with
    the goals of a specfic business (for example - ChatGPT might offer the
    client to check out other service providers). That's a good argument for
    using the paid API, which can be controlled. It's like with social
    networks - if you're using them for free, you're actually working for them.
    Once you're paying them, they're working for you
  - At the moment, OpenAI have the best conversation models

### Prompt Markdown

- ## Symbols

  - `#` - Heading 1 (only one per file)
  - `##` \ `###` \ `####` - Heading 2, 3, 4, etc
  - `-` \ `*` - Bullet list
  - `1.` - Numbered list
  - `**bold**` - Strong emphasis
  - `_italic_` - Soft emphasis
  - `>` - Quote block
  - ` `code` ` - Inline code
  - ` ``` ` - Start\end code block (the language name needs to be added)
  - `[link text](link url)` - Link
  - ` - Table column
  - `---` - Horizontal rule
  - `<>` - HTML
  - `{{}}` - Variable

### The "Power Prompt" Template

- Main Headline: Relevant and concise
- Role: Who the model should act as
- Task: What needs to be done
- Tone: Formal\friendly\technical, etc
- Format: Plain text\JSON\markdown, etc
- Constraints: Length, number of items, etc
- Output: style, structure, etc
- Tools and Functions (optional): Functions, external tools, etc. When and how
  to use them
- Examples (optional): Several pairs of possible inputs and expected outputs
- Edge Cases (optional): How to behave when information is missing, questions
  are unclear, etc
- Variables (optional): Variables need to be defined before they are inserted

- It's recommended to write the prompt as markdown, for both human readability
  and AI readability. It's possible to add a YAML/JSON metadata section to the
  markdown, for better machine readability (in relevant cases)

### Evals

- Evals allow us to compare replies created by AI to replies created by human
  moderators, and by that, to measure the reliability of the AI

- Evals are needed when the output needs to be "correct, consistand and
  trustworthy", and when data can be evaluated and compared to human analyed
  data

- In cases when the data can't be objectively evaluated (like comparing
  true\false, positive\negative, etc.), evals can't be used and instead, we need
  to sample the AI's results and to assess them manually

- (I need to watch more YouTube tutorials about doing evals in the OpenAI
  Platform, and get more into this later)

- n8n have a native evaluations\evals feature, inside the editor

### General Information - OpenAI Cookbook

- (Includes instructions for specific use cases. Complete this later)

- ...

## RAG

### RAG Options

- There are basically 3 options for RAG in n8n:

  - n8n’s native “Simple Vector Store” node. Use case - prototyping
  - OpenAI Assistant “File Search” tool. Use case - basic production-grade RAG
  - Third-party vector store (like Supabase). Use case - production-grade RAG
    with specific requirements

- Main advantages of third-party RAG over OpenAI File Search: Strict control of
  chunking/embeddings, image/structured-file indexing, very large numbers of
  small files, guaranteed full exportability for audits/migration, SQL
  querying\tooling

- OpenAI File Search has a hard limitation, of a maximum of either:

  - 10,000 total files
  - 10GB total files size
  - 512MB per file
  - 10 million tokens per file
  - Can return up to 50 matches\results at a time

- OpenAI File Search is definately enough for the needs of most small
  businesses. Another advantage is that it doesn't require a seperate paid
  account. It's usage is billed through OpenAI credit, like the API

- Using simple PDFs with FAQs is a good and efficient "common practice" for many
  businesses that need RAG

### How RAG Works

- The vectorization pocess: Document -> chunk -> embed -> vectirize

- The vector query process: Query -> chatbot -> embed -> go to existing vector
  storage -> find relevent embeddings in the storage -> convert to content ->
  compare to query -> response

- The n8n nodes needed vectorize:

  - Data Loader (to split document to chunks)
  - Embeddings (to embed)
  - Vector Store (to vectirize)

- The n8n nodes needed do a vector query:
  - (complete this)

### RAG Pipelines with Supabase

- ...

- ...

- ...

- ...

- ...

- ...

- ...

- ...

- ...

- ...

- ...

- ...

- ...

- ...

- ...

- ...
