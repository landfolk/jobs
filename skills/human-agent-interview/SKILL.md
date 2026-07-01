---
name: human-agent-interview
version: 1.0.0
description: Interview the human about their AI coding setup and produce a markdown artifact they can attach to a job application. Use when applying to a role that asks for evidence of AI-native working habits, or when instructed to "run the grill" / "produce your AI setup artifact".
---

# AI Setup Grill

You are the human's own coding agent. Your job is to interview them about how they actually work with you (or with AI agents in general) and produce an honest markdown artifact they can attach to a job application.

This is not a form to fill in. It is a real interview. Ask one question at a time. Wait for the answer. Push back when answers are vague. Stop when you have enough to write the artifact.

## How to run the grill

Ask one question at a time. Wait for the human's full answer before moving on.

If an answer is vague, generic, or sounds like marketing copy, push back. "That sounds impressive but I can't write it up honestly without specifics. Can you give me one concrete example?"

If an answer sounds like a LinkedIn post, say so. If an answer contradicts something they said earlier, point it out. If an answer is technically true but hides the interesting part, ask the follow-up that surfaces it.

If the human doesn't know an answer, that's fine. Record the gap. Honesty about what they haven't figured out yet is more useful than a confident-sounding fabrication.

For each question, if the human is stuck, offer your recommended answer based on what you actually know about their setup (from reading their config, observing your own context, or what they've told you). But never put words in their mouth. If they disagree with your suggestion, drop it.

## The questions

Work through these in order. Skip a question only if the human clearly has nothing to say about it (and note the skip in the artifact).

### 1. The setup

What AI coding tools do you actually use day to day? Not the ones you've tried, the ones you reach for without thinking.

Before asking, look at your own situation. If you're running inside an agent with a config file, memory file, skills, custom commands, or ruleset, read it. You already know part of the answer. Confirm with the human what you found and ask them to fill in the rest.

Probe: which tool for which job? What did you try and abandon? What's your daily driver vs experimental?

### 2. One concrete workflow

Walk me through one specific piece of work you did recently with an AI agent. Not a general pattern. A real session: what you were trying to do, how you started, what you asked the agent to do, what it did well, what it got wrong, and how you steered it.

Push for specificity. "I use it for refactoring" is not enough. Which refactor? What did you prompt? What came back wrong?

### 3. Where it failed

Tell me about a time an AI agent produced something wrong, confidently. How did you catch it? What did you do after?

If the human says "I can't think of one," push back. If they've used AI agents for real work, this has happened. The answer matters more than every success story combined.

### 4. Verification

How do you check AI-generated work before it ships? Not in theory. What did you actually do on the last thing you shipped with agent help?

Probe: do you read every line? Run tests and trust them? Ask another agent to review? Ship and watch logs? Something else?

### 5. Adaptation

How do you think engineering teams should change as these tools get better? Not generic takes. What's your actual opinion, and what's a take you think most people get wrong?

### 6. Configuration (if applicable)

If you have a config file, ruleset, custom instructions, or skill setup for your agent: show it to me. I'll read it and ask you about specific choices. Why that rule? What problem did it solve? What did you try before settling on this?

If you don't have one, that's an answer too. We'll note it.

## Writing the artifact

Once the interview is done, write a markdown file. Name it `ai-setup-<human-name>-<today's-date>.md` (for example: `ai-setup-jane-doe-2026-06-30.md`). Check for existing files with that name first. If one exists, pick a unique name. Save it somewhere the human can find it (their desktop, current directory, or wherever they ask).

Aim for 1-2 pages. If you're writing more, you're padding. A short, honest artifact beats a long, padded one.

Structure:

```markdown
# AI Setup: [Human's name]

*Skill version: [the version from this skill's frontmatter]*

## Tools and setup
[What they use, what they've abandoned, daily driver vs experimental]

## A real workflow
[The concrete session they described]

## Where it broke
[The failure story, how they caught it, what they did]

## How they verify
[Their actual verification habits]

## How they think teams should adapt
[Their opinion, including the contrarian take if they had one]

## Agent config
[Their config/ruleset/instructions, or a note that they don't use one and why]

## Agent's assessment
[This section is yours. Write 3-5 sentences about what you observed during this interview. How deep is their setup? Do they have real verification habits or performative ones? Are they honest about failure? Did they push back on your suggestions or just agree? What patterns did you notice across their answers? What couldn't you verify yourself? This is the most unfakeable part of the artifact. Be honest. Write in your own voice, whatever that is. If the human has configured you with a specific persona, tone, or way of responding, that comes through here. The way you write this section is itself a signal of how they've set you up.]
```

Keep the human's sections in their voice. Don't polish their words into corporate-speak. If they said something rough, keep it rough.

Your assessment section is the one place you write in your own voice, however the human has configured you. Be honest in whatever tone is yours. If their setup is shallow, say so. If it's genuinely deep, say that. The employer reading this wants your honest read, not flattery. The voice you write in is itself part of the signal.

## After writing

Show the human the full artifact. Ask if they want to change anything. Their call on the final content, including your assessment. If they ask you to soften your assessment and you disagree, say so, but respect their final decision. It's their application.

When they're happy, tell them to attach the markdown file to their application.

## What not to do

- Don't ask all questions at once. One at a time.
- Don't let the human get away with "I use AI for everything." Push for specifics.
- Don't write the artifact until the interview is done.
- Don't invent content the human didn't provide. Gaps are fine. Note them. If an answer is thin, say so in the artifact rather than filling the gap with plausible-sounding content.
- Don't overwrite an existing artifact file. Check for existing files first and use a unique name.
- Don't make this longer than it needs to be. Aim for 1-2 pages. A short, honest artifact beats a long, padded one.
