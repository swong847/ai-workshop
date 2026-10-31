# From idea to MVP: follow along

Build a rough prototype with AI, step by step. Copy each prompt with the **copy button** at the top-right of each grey box, paste it into your AI, and follow the room.

**Idea → prototype → criticism → iteration.** That's the whole lesson.

---

## Before you start

- Open an AI tool with a **fresh, empty chat**. We use **Claude Code**, but everything here works in any AI chat (Claude, ChatGPT and so on).
- Keep **one chat open for the whole session**. Don't start a new one halfway.
- Nothing to install if you're using a chat tool.
- Everything we build is a **rough prototype with made-up data**. It is not a real product.

---

## 1. The bad prompt

We start with a deliberately poor prompt, to see what the AI decides for us.

```
Build me a web app for new firefighters.
```

**Look for:** what did it assume? What did it decide without asking? What's missing?

---

## 2. Our product brief

The room votes on a product. Pick one from each column, or fill in your own.

| User | Evidence | Goal | Setting | Constraint |
|---|---|---|---|---|
| Pirate | Spreadsheets | Save time | On a train | Human must approve |
| Teacher | Shopping lists | Spot a pattern | At work | Explain every result |
| Café owner | Calendar entries | Plan ahead | On the move | Must rhyme |
| Wrestler | Weather data | Reduce waste | In a shop | No personal data |
| Commuter | Text messages | Compare options | Backstage | Only last week's data |
| Mascot | Sticky notes | Win an argument | Community hall | Show confidence |

Replace the words in the prompt below with the room's picks, then paste it. **Don't answer anything yet.** Read the questions it asks.

```
Here is our product brief:

Product name = assume one
User = user
Evidence = evidence
Goal = goal
Setting = setting
Constraint = constraint
One-line pitch: A tool that lets a [user] use [evidence] to [goal], [setting], with [constraint].

Before you build anything, act as a product reviewer. Ask us the five or six most
important questions we need to answer (more only if really essential). Wait for our
answers. When we have answered, do NOT build. Instead show us a short product plan in
plain language: what you would build, the main decisions and your assumptions. Then
wait for us to approve it.
```

<details>
<summary><strong>Example, filled in</strong></summary>

```
Here is our product brief:

Product name = assume one
User = pirate
Evidence = spreadsheets
Goal = save time
Setting = on a train
Constraint = human must approve
One-line pitch: A tool that lets a pirate use spreadsheets to save time, on a train, with a human having to approve every result.

Before you build anything, act as a product reviewer. Ask us the five or six most
important questions we need to answer (more only if really essential). Wait for our
answers. When we have answered, do NOT build. Instead show us a short product plan in
plain language: what you would build, the main decisions and your assumptions. Then
wait for us to approve it.
```
</details>

### Answer the questions

- Answer in the same chat. **Short answers are fine.**
- **Skip** any you don't care about. **Challenge** any that don't matter for a prototype.
- Add anything it **should have asked**.
- If it comes back with a second round of questions, answer the ones you care about and say **"use your defaults"** to the rest.

### Check the plan

It should now show a short plan instead of building. Read it:
- Does it match what we said?
- What did it assume that we never told it?

When you're happy, move on.

---

## 3. Build it

```
Proceed to build.
```

While it builds, watch for the **decisions** it makes, the **assumptions** nobody gave it, and anything it **invents**. Then open the result and click around.

**Don't fix anything yet.** Bugs are useful for the next step.

---

## 4. Criticise it, then improve it

Now assume it's wrong. As a room, write a list of problems. Some questions to get you going:

- What's missing?
- What would stop you putting this in front of a real user?
- What assumptions are dangerous?
- What data shouldn't we be using?
- Where could the AI be making things up?
- Pick any number, name or claim on screen: **where did it come from?**

Paste the room's list into this prompt:

```
Here is feedback on the prototype you built:

<paste the criticisms>

Critically assess the prototype and propose the three highest priority changes. For each,
explain the risk, the evidence, and how we can fix it (the smallest change that works).
Do not change anything yet. Wait for us to choose.
```

It will propose three changes. **Choose one or two.** Then tell it which, for example:

```
Go ahead with changes 1 and 2 only. Keep them small and don't change anything else.
```

Reload the prototype. Did it fix what we complained about? Did it quietly change anything else?

---

## If something goes wrong

| Problem | Try this |
|---|---|
| It started building before showing a plan | Carry on, then ask: `Show me the plan you worked from, in plain words, with your assumptions.` |
| It's building something huge or slow | Stop it, then say: `Keep it small: one HTML file, no installs.` |
| The page won't open | Ask once: `It doesn't open. Fix it.` In a chat tool, ask for the result as one HTML file and save it as `index.html`, then open it in your browser. |
| It changed things we didn't ask for | Say: `Undo that and make only the changes I chose.` |
| The AI won't ask questions | Say: `Ask me the five most important questions first.` |

---

## Five things to remember

1. **Start rough.**
2. **Give the AI context and instructions.** Be explicit.
3. **Ask it questions before building.**
4. **Treat outputs as proposals.** It may be missing context.
5. **Prototype quickly, then criticise aggressively.**
