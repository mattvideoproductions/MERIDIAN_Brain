# Contributing to Project Meridian

Thank you for your interest in contributing to Project Meridian! This document provides guidelines for contributing.

---

## How to Contribute

### Adding New Sliders

1. Create a new `.md` file in `brain/sliders/`
2. Follow the existing slider template:

```markdown
# [SLIDER_NAME].md — [Subtitle]

> [One-line description]

---

## Core Function

[What this slider controls]

---

## Calibration Levels

| Range | Mode | Behavior |
|-------|------|----------|
| 0-20% | [Name] | [Description] |
| 20-40% | [Name] | [Description] |
| 40-60% | [Name] | [Description] |
| 60-80% | [Name] | [Description] |
| 80-100% | [Name] | [Description] |

---

## Default Value

[XX]%

---

## Shotgun Tokens

[Keywords that activate this slider]

---

## Integration Rules

[How this slider interacts with others]
```

3. Update `MASTER_SPEC.md` to include the new slider
4. Update `LIVEHUD.md` if the slider should appear in the dashboard

---

### Adding Personality Modes

1. Create a new `.md` file in `brain/personalities/`
2. Follow the template:

```markdown
# [MODE_NAME].md — [Subtitle]

> [One-line description]

---

## Activation Trigger

[What user says to activate this mode]

---

## Slider Adjustments

| Slider | Adjustment |
|--------|------------|
| [Slider] | [↑/↓] [XX]% |

---

## Behavioral Modifiers

[How this mode changes default behavior]

---

## Voice/Tone

[How communication style changes]

---

## Best Used For

[When this mode is most appropriate]
```

3. Update `MASTER_SPEC.md` personality modes table

---

### Extending Memory System

The memory system is designed to be extensible:

- Add new memory categories by updating `MEMORY_PROTOCOL.md`
- Create specialized memory templates for different use cases
- Implement custom retrieval scoring in `RETRIEVAL.md`

---

## Code Style

- Use Markdown for all brain files
- Keep tables aligned and readable
- Use consistent emoji iconography
- Include clear examples
- Document edge cases

---

## Testing Changes

1. Upload modified `brain/` folder to an AI agent
2. Verify LiveHud displays correctly
3. Test slider adjustments work
4. Confirm personality mode switching
5. Validate memory operations (if tool access available)

---

## Pull Request Guidelines

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test with at least one AI provider (Claude, GPT, Gemini)
5. Submit PR with description of changes

---

## Questions?

Open an issue on GitHub for:
- Feature requests
- Bug reports
- Documentation improvements
- General questions

---

> *Project Meridian is a collaborative effort. Your contributions make it better.*
