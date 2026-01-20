# Festival Operations Skills for Goose

A collection of skills that teach [Goose](https://github.com/block/goose) how to handle winter festival operations. Built as part of the [Goose Advent Challenge Day 14](https://github.com/block/goose/discussions/6170).

## What are Skills?

Skills are markdown files with YAML frontmatter that give Goose domain expertise. When Goose starts a session, it discovers available skills and can load them when relevant.

## Skills Included

| Skill | Description | Expert |
|-------|-------------|--------|
| `festival-operations` | Master guide covering all operations | All team |
| `festival-customer-experience` | Customer service and line management | Madame Zelda |
| `festival-security` | Security protocols and vendor management | Marcus |
| `festival-lost-found` | Lost & found procedures | Maria |
| `festival-communications` | Marketing, press, and emergency comms | Elena |

## Installation

Copy the skill folders to your Goose skills directory:

```bash
# Linux/macOS
cp -r festival-* ~/.config/goose/skills/

# Windows (PowerShell)
Copy-Item -Recurse festival-* $env:USERPROFILE/.config/goose/skills/
```

## Usage

Start a Goose session and the skills will be automatically available:

```bash
goose session
```

Then ask questions like:

- "What skills do you have?"
- "A vendor is playing music too loud. What should I do?"
- "A kid lost their stuffed animal - help!"
- "A reporter wants to interview me about the festival"
- "What's the opening checklist?"

You can also explicitly request a skill:

```bash
"Use the festival-security skill to help me handle this vendor complaint"
```

## Skill Structure

```
festival-operations/
├── SKILL.md                    # Main skill definition
├── checklists/
│   ├── opening.md              # Pre-opening checklist
│   └── closing.md              # End-of-day checklist
└── templates/
    └── incident-report.md      # Incident report template

festival-customer-experience/
└── SKILL.md

festival-security/
└── SKILL.md

festival-lost-found/
└── SKILL.md

festival-communications/
└── SKILL.md
```

## Key Features

### Emergency Codes (from Security skill)
- **Code Yellow** - Lost child
- **Code Blue** - Medical emergency
- **Code White** - Weather emergency
- **Code Orange** - Suspicious activity

### Vendor Noise Complaint Protocol
1. Verbal warning (1st offense)
2. Written warning (2nd offense)
3. Shutdown (3rd offense)

### Lost & Found Patterns
- Ice rink → mittens and scarves
- Food court → phones and wallets
- Kids areas → stuffed animals (URGENT!)

## Claude Desktop Compatibility

These skills also work with Claude Desktop! Place them in `~/.claude/skills/` for cross-tool compatibility.

## License

MIT License - Feel free to use, modify, and share!

## Acknowledgments

Built with [Goose](https://github.com/block/goose) by Block.
