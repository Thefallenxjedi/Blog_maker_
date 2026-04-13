# Project Specification — SEO Blog Generation Agent

This file defines the architecture and workflow for the SEO Blog Generation Agent.

The system generates **SEO optimized blogs in strict Chatzy blog format** using automated research and structured writing.

---

# System Goal

The system automatically generates a complete blog article based on a topic provided by the user.

The blog must:

* Follow the strict Chatzy blog format
* Include metadata fields
* Include structured sections
* Include a Chatzy AI closing section
* Include FAQ
* Include an SEO keyword schema block

The output must be **publish-ready MDL format**.

---

# User Input

The user provides:

```
Blog Topic
```

Example:

```
AI voice agents
```

or

```
AI customer support automation
```

---

# System Output

The system produces an **MDL blog file** containing:

1. Metadata block
2. Blog title
3. Blog content sections
4. Closing automation section
5. FAQ section
6. SEO keyword JSON-LD block

The output must follow the structure defined in `instructions.md`.

---

# Workflow Stages

The system follows a multi-step workflow.

## Stage 1 — Topic Analysis

Input:
User topic

Tasks:

* Understand the topic
* Expand into related concepts
* Identify possible blog angles

Output:
Topic understanding

---

## Stage 2 — Web Research

The system searches the internet for:

* Top ranking blogs
* Common headings
* Popular keyword usage

Goal:
Understand how competitors structure content.

---

## Stage 3 — Keyword Discovery

The system identifies:

Primary keyword
Supporting keywords
Long-tail keywords

These keywords guide the blog content.

---

## Stage 4 — Blog Strategy

The system determines:

* Blog title
* Blog structure
* Section order
* Key points to include

This ensures the blog is optimized for SEO.

---

## Stage 5 — Blog Generation

Using the strategy and instructions, the agent generates:

* Metadata
* Introduction
* Blog sections
* Tool references
* Implementation steps
* Best practices
* Closing section
* FAQ
* SEO keyword schema

The structure must strictly follow `instructions.md`.

---

# Tools Used

The workflow uses the following capabilities:

Web search
Large language model reasoning
SEO keyword extraction
Content generation

These tools help produce optimized blogs.

---

# File Storage

Generated blogs should be saved as MDL files (`.mdl`).

Example path:

```
/blogs/{slug}.mdl
```

Example:

```
/blogs/ai-voice-agents.mdl
```

---

# Deployment Environment

The system runs inside the **Antigravity agent workflow environment**.

The agent orchestrates:

Topic input
Research
Keyword extraction
Content generation

The output is returned as an MDL file.

---

# Definition of Done

The system is complete when:

* The agent accepts a blog topic
* Performs research
* Identifies keywords
* Generates a structured blog
* Follows Chatzy blog format
* Produces publish-ready MDL files

No manual formatting should be required.

---

# Future Improvements

Possible upgrades include:

* Automatic cover image generation
* Internal linking suggestions
* SEO score validation
* Automatic publishing to CMS
* Blog outline suggestions

These features can be added after the core workflow is stable.
