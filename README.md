# weekly-reading

A curated weekly reading list of 20 papers (5 each in Bayesian statistics,
measurement theory, target trial emulation, and information geometry), selected
for depth, craft, and originality rather than popularity. The list is produced
once a week by an asynchronous agent.

## Layout

```
briefs/
  YYYY-MM/
    MM-DD-YY.md      Dated weekly brief: 20 picks grouped into threads, plus a synthesis.
reading-log.md       Cumulative ledger of every paper ever recommended. The dedup
                     source of truth: the agent reads it each run and never repeats a title.
weekly-reading-list-prompt.md  The recurring agent prompt (the spec for how lists are built).
good-paper-sites     Running list of sources with good-quality papers.
```

## How it works

Each run, the agent reads `reading-log.md`, hunts for gems per the rules in
`weekly-reading-list-prompt.md`, writes a dated brief to
`briefs/YYYY-MM/MM-DD-YY.md`, and appends its 20 picks to `reading-log.md`.

Briefs are organized into month folders (`briefs/2026-06/`) so they sort
chronologically and stay tidy across the year.
