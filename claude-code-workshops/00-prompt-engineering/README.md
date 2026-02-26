# Prompt Engineering

Before diving into files and tools, this module covers the most fundamental skill: writing better prompts. A basic prompt gets a basic answer. This module shows how to use Claude to improve your own prompts — and why the difference matters.

**Files used:** None
**Prerequisite:** Claude Code installed and running

## How this works

Claude is a reasoning system — the quality of its output is directly shaped by the quality of its input. A vague prompt produces a vague answer not because Claude is limited, but because there isn't enough context to do better. The good news: you can ask Claude to help you build a better prompt, and it will tell you exactly what context it needs.

## Step 1: Try a Basic Prompt

Start with something simple:

```
Explain Generative AI
```

You'll get a reasonable answer — a solid paragraph or two covering the basics. It's not wrong, but it's not particularly useful either. It's the answer Claude gives when it has no idea who you are, what you need, or why you're asking.

## Step 2: Ask Claude to Help You Improve It

Instead of asking Claude to blindly rewrite your prompt, ask it to gather context first:

```
I want a better answer to that question. Before rewriting my prompt, ask me a few questions to understand my context.
```

Claude will ask things like: Who is the audience? What's the purpose? How technical should it be? What format would be most useful? What will you do with the answer?

Notice what Claude is asking for — this is the anatomy of a good prompt.

## Step 3: Answer the Questions

Answer based on your actual situation. Be specific: who will read this, what decision or action does it need to support, and what format works for your context.

## Step 4: Run the Improved Prompt

Claude will rewrite your prompt incorporating your answers. Run it and compare the result to Step 1.

The difference isn't subtle.

## Step 5: Harness It

Steps 1–4 showed that better context produces better output. But you had to provide that context manually, in the moment. A **harness** makes it persistent — so every session starts with the right context already in place, and every response is shaped by it.

Claude Code reads `CLAUDE.md` files automatically at the start of every session. You write down the context that matters — your role, your conventions, how you want things done — and Claude loads it before you type anything. The key principle: **only include things Claude can't figure out on its own**. Your role and preferences, yes. Standard conventions it already knows, no.

Ask Claude to create one based on your conversation:

```
Based on everything I've told you about my context, create a CLAUDE.md file that captures my role, what I'm working on, and how I want responses structured.
```

Claude will generate a configuration file in your working directory. Every subsequent session starts with your context already loaded. For technical projects, you can also use `/init` to bootstrap from your codebase.

Claude Code supports layered configuration — a shared `CLAUDE.md` checked into version control for your team, plus a personal `CLAUDE.local.md` for your own preferences. More specific files take precedence. Treat your configuration like any shared document: review it when things go wrong, prune it regularly, and refine it as your work evolves.

## What You Learned

- A basic prompt gets a basic answer — not because Claude is limited, but because context is missing
- Asking Claude to ask *you* questions reveals exactly what makes a prompt good
- A `CLAUDE.md` file harnesses that context permanently — every session starts with it already loaded
- Only include what Claude can't figure out on its own, and refine it over time

> **Try more:** Create a `CLAUDE.md` for your actual work. Start with your role and one or two preferences, then refine it over a few sessions.

---

[Next: Document Analysis →](../01-document-analysis/README.md)
