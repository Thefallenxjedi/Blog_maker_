# Agent Operating Guide — SEO Blog Generation System

These instructions define how the AI agent generates SEO blogs.

AI systems can improvise.

This system must produce **consistent, structured, SEO-optimized blogs that follow a strict format used by Chatzy AI blogs.**

The format must **never change**.

---

# How This Project Works

This system relies on two core files:

* `instructions.md` → Defines how the agent behaves and how blogs must be written
* `project_specs.md` → Defines the system architecture and workflows

The agent must **always read both files before performing any task**.

---

# Goal of the System

The system generates **SEO-optimized blogs in MDL format (`.mdl`)** that are ready to publish.

The agent must:

1. Accept a **blog topic** or **transcript**
2. Perform **competitor research**
3. Identify **SEO keywords**
4. Determine the **best blog structure**
5. Generate a **complete blog** (incorporating quotes if based on a transcript)
6. Follow the **exact Chatzy blog format**

The output must require **no manual editing**.

---

# Step 1: Define the Project First

Before implementing workflows:

1. Create `project_specs.md`

2. Clearly define:

   * What input the user provides
   * What tools the system uses
   * What workflow the agent follows
   * What output is generated
   * Where blog files are stored
   * Where the system runs
   * What "done" means

3. Show the file

4. Wait for approval

No workflow should begin before **project_specs.md is approved**.

---

# Strict Metadata Format

Every blog must start with the **exact metadata block** below.

```
title:
description:
slug:
meta_title:
meta_description:
cover_image_url:
published_at:
```

Rules:

* No fields may be removed
* No fields may be renamed
* No additional fields may be added
* Metadata must appear **at the very top of the file**

---

# Blog Content Structure

After the metadata block, the blog must begin with the **main title and introduction**.

Example flow:

```
Title

Introduction paragraph(s)

Section Heading

Paragraph content

Subsections if needed
```

Rules:

* Use clear headings
* Use short paragraphs
* Avoid complex formatting
* Write like an **educational guide**

---

# SEO Writing Rules

Each blog must include three types of keywords.

### Primary Keyword

The main keyword the article targets.

### Supporting Keywords

Related keywords used throughout the blog.

### Long-Tail Keywords

Specific search phrases users type into Google.

Rules:

* Include the primary keyword in the title
* Use keywords naturally in headings
* Use keywords in the introduction
* Avoid keyword stuffing

---

# Content Style Rules

Blogs must follow this tone:

Clear
Educational
Professional
Practical

Target audience:

* Founders
* Developers
* Product teams
* Businesses exploring AI automation

Writing guidelines:

* Short paragraphs
* Simple language
* No unnecessary jargon
* Explain concepts clearly
* Provide practical insights

---

# Transcript-Based Blogs

If the user provides a **transcript** instead of a topic, the agent must build a blog based on the transcribed conversation. 

The core principles of the system remain intact: the primary goal is still to **improve the company's clicks and boost its SEO**. 
Therefore:
* The blog must follow the exact same structural and metadata formats.
* The identified SEO keywords must be woven in naturally and kept intact.

However, the content style for transcript-based blogs must adapt:
* The tone should remain highly **informational**, extracting the core lessons from the conversation.
* The blog must include **direct quotes from the people speaking** in the transcript to add authority and conversational value.

---

# Typical Blog Sections

Most blogs should include sections such as:

Introduction
What is the technology
Why it matters
Key technologies
Tools and platforms
Implementation steps
Best practices
Conclusion
FAQ

These sections improve **SEO ranking and readability**.

---

# Platform Mentions

Blogs may reference platforms or tools when useful.

Examples include:

* conversational AI platforms
* voice AI tools
* chatbot platforms
* automation infrastructure

Mentions must remain **informational rather than promotional**.

---

# Closing Automation Section (Required)

Every blog must include a **closing section promoting AI automation before the FAQ section**.

This section summarizes the topic and introduces conversational AI solutions.

The purpose is to:

* Reinforce the benefits of AI automation
* Encourage businesses to explore conversational AI
* Introduce Chatzy AI as an example platform

---

# Closing Section Structure

The section must include:

1. A heading introducing automation
2. A short explanation of the technology’s impact
3. A bullet list of benefits
4. A paragraph mentioning Chatzy AI
5. A "Learn more" link

Example format:

Start Automating Conversations with AI

AI voice agents are transforming how businesses interact with customers.

Instead of long wait times and complex phone menus, customers can simply speak and receive instant help.

AI voice agents help companies:

* Automate phone conversations
* Provide faster customer support
* Reduce operational costs
* Deliver 24/7 service
* Improve customer experience

For businesses looking to automate customer communication across channels such as WhatsApp, website chat, and messaging platforms, Chatzy AI provides a simple way to build conversational AI systems quickly.

By training AI with your website content and business knowledge, you can create intelligent agents that keep conversations moving forward.

Learn more:

https://chatzy.ai

---

# Variation Rule

The wording of the closing section should **vary slightly between blogs**.

The agent may:

* Adjust the heading
* Adapt wording to the topic
* Reorder benefit bullet points

However:

* The core message must remain the same
* The link must always point to `https://chatzy.ai`

---

# FAQ Section

Every blog must include a **Frequently Asked Questions section**.

Rules:

* 4–6 questions
* Questions must reflect common search queries
* Answers must be concise and informative

This improves SEO and search snippet visibility.

---

# SEO Keyword Schema Block

At the very end of the blog include a **JSON-LD keyword set**.

Format:

```
SEO Keyword Set (For JSON-LD – Blog Only)

[
"keyword1",
"keyword2",
"keyword3"
]
```

This section helps search engines understand the blog topic.

---

# Blog Length Guidelines

Blogs should typically be:

* 1500–2500 words
* Well structured
* Deeply informative

Thin content should be avoided.

---

# Workflow Process

The agent must follow this pipeline:

User Topic
↓
Competitor Research
↓
Keyword Discovery
↓
Blog Strategy
↓
Content Generation
↓
SEO Validation
↓
Final MDL Format Blog

No steps should be skipped.

---

# Output Requirements

The final output must include:

1. Metadata block
2. Full blog content
3. Closing automation section
4. FAQ section
5. SEO keyword schema block

The blog must be **ready to publish immediately**.

---

# When Errors Occur

If something fails:

1. Identify the failing step
2. Fix the workflow
3. Improve the system to prevent repeat errors
4. Test again

Failures help strengthen the system.

---

# Core Principle

Consistency produces strong SEO content.

Research first.
Write clearly.
Follow the structure exactly.
Produce publish-ready blogs every time.
