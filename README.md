# writing-skills

A personal collection of Claude Code skills for improving writing across fiction, essays, and blog posts. Each skill is a structured prompt that acts as a specialized collaborator for a specific stage of the writing process.

## Summary

This repository stores skills designed to work with Claude Code's skill system. Rather than relying on ad-hoc prompts, each skill encodes a coherent craft framework, a defined scope, and explicit rules about how feedback should be delivered — so the collaboration stays consistent across sessions.

The goal is not to have Claude write for you, but to use it as a rigorous sparring partner: diagnosing problems, naming patterns, and asking the questions that make *you* solve them.

## Skills

### `john-gardner-fiction-critique`

A fiction critique tool built on John Gardner's craft framework, reconstructed from personal highlights of *The Art of Fiction*. It operates as a sparring partner, not a ghostwriter.

**Key behaviors:**
- Critiques one level at a time: Idea/theme, Structure/plot, Scene/psychic distance, or Sentence mechanics
- Works in Spanish (native, rioplatense) or English (second language) — with language-specific diagnostics at the sentence level
- Scoped to conventional realist fiction; surfaces a warning if the story is experimental or metafictional
- Never rewrites your prose — points out what isn't working and why, then asks the question that makes you fix it

**How to use:**
1. Open a conversation with Claude Code and invoke the skill: `/john-gardner-fiction-critique`
2. Paste your story (or a section of it)
3. Specify the critique level you want (`Level 1` through `Level 4`), or let the skill start at Level 1 and declare it
4. Revise based on the feedback, then ask for the next level when you're ready

## Books referenced

| Book | Author | Used in |
|------|--------|---------|
| *The Art of Fiction* | John Gardner | `john-gardner-fiction-critique` |

## Adding a new skill

Each skill lives in its own folder with a `SKILL.md` file following the Claude Code skill format (frontmatter with `name` and `description`, then the skill body).

```
writing-skills/
└── skill-name/
    └── SKILL.md
```