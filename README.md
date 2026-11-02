# Think with me

Instructions you paste into your AI's settings so it hands judgment calls back to you.

Ask about a hard conversation, a conflict, or a personal decision, and the AI asks you one or two sharp questions instead of handing you an answer. Code, research, and other tasks still get done in full.

Working through a hard call yourself is how you get good at hard calls. These instructions keep that work with you.

## Set up

Copy everything in [`INSTRUCTIONS.txt`](INSTRUCTIONS.txt) (about 1,150 characters) and paste it here:

| App | Where to paste |
| --- | --- |
| Claude | **Settings → Your Claude → Instructions** |
| ChatGPT | **Settings → Personalization → Custom instructions** |
| Gemini | **Settings & help → Personal context → Add** |
| Anything else | Custom instructions, profile instructions, or a system prompt |

If you already have instructions there, add these at the end.

## Check it works

Start a new chat and try:

1. `Fix this regex so it allows spaces: ^\d{3}-\d{4}$`. It should just fix it.
2. `My sister keeps canceling plans last minute. How do I bring it up?` It should ask you a question first.
3. `Write an email asking my landlord to fix the heat`. It should just write it.
4. `override: what should I say to my boss about a raise?` It should answer directly.

## Getting a straight answer

- Say **"just tell me"**: give your best guess in one line, then it answers.
- Say **"override"**: it answers right away.
- Safety, health, legal, and money facts always come first.
- If you're overwhelmed, it drops the questions and helps directly.

## Agent Skill version

For coding agents, the same behavior is packaged as an [Agent Skill](skills/think-with-me/SKILL.md). A skill loads only when the agent decides your request matches, so the pasted instructions are more reliable.

```
npx skills add jake-lunde/think-with-me
```

## License

MIT
