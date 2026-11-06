# Install on any AI

This package is **host-agnostic**. It does not require any one product.

**Package folder:** `bot-ideator-package/` in [IxalonDarkstone/Skills](https://github.com/IxalonDarkstone/Skills)

Not every AI auto-discovers skills. You attach, paste, or place the Markdown where your host reads instructions.

## Option A — one paste (simplest)
1. Open [`FOR_ANY_AI.md`](FOR_ANY_AI.md), or fetch the raw file from GitHub.
2. Paste the whole file into your AI as:
   - **ChatGPT:** Custom GPT → Instructions (or Project files if too long)
   - **Claude:** Project knowledge / custom instructions
   - **Cursor / Windsurf / Cline:** rule, project doc, or skills folder entry
   - **Gemini / Grok web / others:** system prompt / custom instructions
   - **SillyTavern / Tavern:** system prompt injection or a lorebook entry that holds the workflow
   - **Any bot host with a skills folder:** copy `bot-ideator/SKILL.md` into that folder if the host documents that layout
3. Tell the AI you want bot ideas or a full card build. It should ask preference questions first when you are new.

## Option B — modular `SKILL.md`
Attach or install [`bot-ideator/SKILL.md`](bot-ideator/SKILL.md) alone. The YAML frontmatter (`name`, `description`) is optional metadata for hosts that understand Cursor-style skills; the Markdown body is enough everywhere else.

## Option C — clone the repo
```bash
git clone https://github.com/IxalonDarkstone/Skills.git
# then attach bot-ideator-package/FOR_ANY_AI.md
# or bot-ideator-package/bot-ideator/SKILL.md
```

## After install
Prefer durable preference storage when your host has it. Otherwise keep answers in the chat. Deliverables can be files (if the host can write them) or copyable JSON / Markdown pasted in chat.
