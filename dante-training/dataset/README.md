# Dante Training Dataset

Raw material for training Dante's emotional intelligence, dating coaching, and relationship intuition.

## Structure

```
dataset/
├── personal/          # Matt's own case studies and experiences
├── friends/           # Anonymized stories from people Matt knows
├── online-threads/    # Reddit, forums, X threads, etc.
└── raw-transcripts/   # Unprocessed voice notes / chat logs before cleanup
```

## File Naming Convention

`[category]-[YYYY-MM-DD]-[slug].md`

Examples:
- `personal-2026-03-27-emily-situationship.md`
- `friends-2026-04-01-long-distance-breakup.md`
- `online-2026-04-05-reddit-ghosting-thread.md`

## Case Study Format

Each file should include:

```markdown
## Metadata
- Source: personal | friend | online
- Tags: [situationship, coworker, avoidant, breadcrumbing, etc.]
- Emotional themes: [attachment, trust, grief, revenge motivation, etc.]
- Outcome: [moved on, reconciled, ongoing, unknown]

## Summary
Brief overview of the situation.

## Key Dynamics
What made this situation complex or instructive.

## Dante Coaching Notes
How Dante should approach someone in this situation.
What to say. What NOT to say. What to watch for.
```

## Sources
- Personal conversations and voice notes → `personal/` or `raw-transcripts/`
- Friends (anonymized) → `friends/`
- Reddit r/dating, r/relationships, r/ExNoContact, X threads → `online-threads/`
