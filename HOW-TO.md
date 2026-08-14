# How to use this

A step-by-step guide. No experience needed. Read it top to bottom.

---

## 1. What is this?

Claude is an AI assistant. Out of the box, it is a generalist. It knows a bit about everything.

A **skill** is a set of instructions you give Claude once. After that, Claude follows those instructions every time they are relevant. You do not have to explain yourself again.

This bundle has **6 skills**. Together they do the job of a copywriting team: they take what you know about your customer and turn it into finished ads, then check the quality.

You do not need to know how to code. You will not write any code. You will copy a file, click some buttons, and then type normal sentences to Claude.

---

## 2. What you need before you start

Pick the one that matches you:

**If you use Claude in a web browser or the Claude desktop app** (this is most people):
- A paid Claude plan. Pro, Max, Team, or Enterprise.
- The file creation setting turned on.
- Free plans cannot add skills. If you are on Free, you need to upgrade, or use the second option below.

**If you use Claude Code** (this is the version that runs in a terminal window):
- Any plan that includes Claude Code.
- Nothing else.

Not sure which one you have? If you talk to Claude in a browser tab at claude.ai, you are the first one.

---

## 3. Get the files

Go to the top of this page and find the green **Code** button. Click it. Click **Download ZIP**.

A file lands in your Downloads folder. Double-click it to open it. You now have a folder with everything in it.

Inside that folder there is another folder called **dist**. It holds 6 small zip files, one per skill. You will use those in a moment.

---

## 4a. Install in the Claude app (browser or desktop)

Do this once per skill. There are 6 skills, so you will repeat this 6 times. It takes about a minute each.

1. Open Claude in your browser or desktop app.
2. Click your name or picture in the bottom left corner.
3. Click **Settings**.
4. Click **Features**.
5. Find the Skills section. Click the button to add or upload a skill.
6. Choose one zip file from the **dist** folder. Start with `brand-brief.zip`.
7. Wait for it to finish. You will see the skill appear in the list.
8. Repeat from step 5 with the next zip file.

**Do not unzip the files in the dist folder.** Upload them exactly as they are. Claude needs them zipped.

When all 6 are listed, you are done.

> **Short on time?** You do not need all 6 to start. Upload `brand-brief.zip`, `creative-copywriter.zip` and `creative-reviewer.zip`. That is enough to write and check ads. Add the rest later.

---

## 4b. Install in Claude Code

Two options. The first is easier.

**Option 1. One command.**

Open Claude Code and type this, then press enter:

```
/plugin marketplace add Sprints-and-Sneakers/creative-copywriting-bundle
```

Then type this and press enter:

```
/plugin install creative-copywriting
```

**Option 2. Copy the folder.**

Copy the `skills` folder from your download into the `.claude/skills` folder inside your project.

Either way, close Claude Code and open it again afterwards. That is what makes the skills show up.

---

## 5. Check it worked

Type this to Claude:

> What skills do you have?

Claude should list them. You are looking for names like `brand-brief` and `creative-copywriter`.

If nothing shows up, jump to section 8.

---

## 6. How to actually use it

You do not type commands. You just ask, in plain English.

Start a new chat and type something like:

> Run the brand brief for my company.

Claude will ask you questions about your business. Answer them honestly. If you do not know an answer, say so. Claude will mark it as unknown instead of making something up.

Then, when you are ready for ads:

> Now write me Instagram ad scripts using that brief.

And to check the quality:

> Review that copy and score it.

And as a last pass before anything goes live:

> Check this copy for typos and AI-sounding writing.

Ask in normal words and the skills switch on by themselves when they are relevant. There is nothing else to learn.

**The order that works best:**

1. Brand brief. Tells Claude about your business.
2. Strategy. Decides what to run, where, and in what mix.
3. Copy. Writes the actual ads.
4. Review. Scores the ads and rewrites the weak ones.
5. Copy check. Catches typos and anything that still sounds like a robot.

You can skip steps. If you already have a strategy, start at step 3.

---

## 7. The one thing that decides if this works

Read this bit twice.

These skills write ads based on what you tell them about your customers. If you tell them very little, you get boring ads that could belong to any company. That is not the AI failing at its job. That is the AI having nothing to work with.

So give it real customer words. Not your summary of what customers think. The words they actually used.

Good things to paste in:
- Reviews people left you, copied and pasted
- Things customers wrote in emails
- Complaints
- What people say on the phone
- Reviews of your competitors

Bad things to paste in:
- "Our customers value quality and service"
- Your website's About page
- A list of your features

The first list is what people really said. The second is marketing language, and marketing language makes weak ads.

If you have 50 real customer sentences, paste them in. The ads will get noticeably better. This is the single biggest lever you have.

---

## 8. When something goes wrong

**The skills do not show up.**
Close Claude completely and open it again. In the app, check Settings and Features to confirm they uploaded. In Claude Code, check you restarted it.

**It says I cannot upload skills.**
You are probably on a Free plan, or file creation is switched off. Check Settings, then Features. Skills need a paid plan.

**Claude ignores a skill.**
Say the name out loud in your message. For example: "Use the creative-copywriter skill to write this." That forces it.

**The ads are boring.**
Go back and read section 7. Almost every time, this is the reason. Give it real customer language.

**Claude asks me questions I cannot answer.**
Say "I don't know" and keep going. The skills are built to handle gaps. They mark unknowns instead of inventing facts.

**I want to start over.**
Open a brand new chat. Old chats keep old context and can confuse things.

---

## 9. Where your work is saved

Claude writes files as it goes. They are organised like this:

```
output/
  your-brand-name/
    01-research/      who your customer is
    02-strategy/      the plan
    03-copywriting/   the actual ads
```

In Claude Code, these appear as real files in your project folder.

In the Claude app, ask Claude to show you the files or give you a download link.

---

## Still stuck?

The research part is the bit we do as a service. That means actually gathering hundreds of real customer quotes and studying competitors properly, which takes time most people do not have.

If you want to do it yourself, we have a second free bundle for exactly that: the **Creative Research Bundle**. It walks you through finding out what your customers actually say, and hands the result straight to these skills.

If you would rather have it done for you, come talk to us at [sprintsandsneakers.com](https://sprintsandsneakers.com).
