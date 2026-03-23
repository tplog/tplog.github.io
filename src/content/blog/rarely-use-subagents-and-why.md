---
title: "Rarely Use Subagents, and Why"
description: "Human cognitive bandwidth is limited. Instead of multithreaded dispatching, reserve it for Socratic steering—stepping outside the frame and asking good questions."
pubDate: "Mar 22 2026"
tags: ["ai"]
---

When collaborating with AI agents, it is easy to fall into a kind of technological fervor: since AI is so powerful, why not spin up multiple sub-agents or use multithreading to process tasks in parallel? Let them write code, search documentation, and run tests simultaneously, while I just sit in the middle acting as a "dispatcher."

It sounds wonderful, but I have been actively resisting this temptation. I insist on not using sub-agents, nor do I engage in parallel dispatching.

The reason is simple: **human cognitive bandwidth is limited.**

When you distribute your limited attention across multiple threads to command agents, you will quickly find yourself lost. You no longer know what the agent on each thread is actually talking about, what its context is, or why it is making its current decisions. Once you lose control over the context, you lose the ability to "steer." And steering is precisely the most core and difficult part of human-machine collaboration.

## The Executor Inside the Frame vs. The Outsider Beyond It

To understand why steering is so crucial, we first need to see through the nature of Large Language Models (LLMs).

The core mechanism of an LLM is predicting the next token. This means that when it generates content, it is strongly constrained by the existing context. If your prompt already implies a certain affirmative assumption (for example: "Can you help me optimize this code?"), then in all likelihood, its next token will be "Yes," and it will run wild down the path of "how to optimize."

**An LLM always operates within a given "frame."** It is exceptionally good at digging deep within a specified frame—it can go very far, very fast, and very comprehensively in one direction. But it will almost never proactively jump out of the frame to question the frame itself. More importantly, it is unaware that it has been locked in by the context.

This is exactly where human intervention is needed.

The greatest value a human can provide in this collaborative relationship is not to execute alongside the AI within the frame, but to **step outside the frame and provide the "outsider" perspective that the AI lacks.**

Perhaps the problem is not "how to optimize this code," but rather "this feature shouldn't be built in the first place." You have the business context, you know the company strategy, you understand user needs, and you can bear the cost of abandonment—these are all things missing from the AI's context.

A good steersman is not the person who knows the most technical details, but the person who **knows when it is time to change the frame.**

## Socratic Steering: Giving Questions, Not Answers

So, how do you effectively steer an agent? The method I advocate is **Socratic steering**.

Socrates himself never said, "Let me tell you what the truth is"; he only asked questions. He believed that knowledge is not instilled from the outside, but is "delivered" (like midwifery) through relentless questioning.

When steering an agent, the worst approach is to give the task directly (for example: "Help me add a version control feature"). This forces the agent to guess out of thin air without a foundation in reality, and the results are often completely off track. A better approach is to ask questions step by step: first let the agent read the relevant code, then ask it what feasible solutions exist, and only finally give the execution command.

Through this method, you hand the responsibility of building context over to the agent itself. It "discovers" reality during the conversation, participates in decision-making, and ultimately executes a task that it understands itself. **Discovered context is real-time and accurate; pre-written documentation is static and prone to rot.**

This also explains why the path of "writing all specifications into documentation and letting the agent read it itself" does not work—documentation rots, the agent drifts, and the time you spend maintaining documentation will eventually exceed the time spent on development itself.

## The Scarcity of Bandwidth Defines the Human Role

Returning to the initial question: why do I refuse multithreading?

Because Socratic steering is fundamentally a **deep dialogue**. It requires you to remember what you asked in the previous round, what the agent answered, and where you should lead it next. This is a chain of thought that demands complete attention; once it branches, the chain breaks. You become an inefficient dispatcher rather than an effective steersman.

Precisely because human cognitive bandwidth is limited, we should be even more reluctant to waste it on multithreaded dispatching and execution within the frame. We should reserve this precious bandwidth for the most important thing: **maintaining the clarity of an outsider, scrutinizing the frame, and asking good questions.**

A single-threaded human + a single-threaded agent are the perfect collaborators with perfectly aligned contexts.

In this era of AI's rapid advancement, acknowledging the limits of our own bandwidth might just be the highest wisdom in mastering AI.
