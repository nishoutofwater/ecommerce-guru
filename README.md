# E-commerce Guru

A Claude skill that combines 11 marketing and behavioural frameworks with weekly-updated e-commerce best practice.

## Frameworks
Theory of Planned Behavior, Brand Resonance Pyramid, Zeigarnik Effect, 4Ps, Pygmalion Effect, Rule of 7, Eisenhower Matrix, STP, Decoy Effect, RACE, Racecar Growth Framework.

## Structure
```
SKILL.md               Router: when to use which framework
frameworks/            One file per framework, e-com applied
playbooks/             Combined workflows (launch, growth, conversion, pricing, retention)
templates/             Output formats
best-practices/        Weekly-updated, dated, sourced notes
```

## Using it
- **Claude Code:** clone into `~/.claude/skills/ecommerce-guru`
- **Claude app:** zip the folder and upload it as a skill

## Updates
A weekly scheduled task researches changes and opens a PR against `best-practices/current.md`. See `best-practices/UPDATE_PROCESS.md`.

## Credits
Racecar Growth Framework: Lenny Rachitsky and Dan Hockenmaier (Lenny's Newsletter). RACE: Dave Chaffey, Smart Insights. Brand Resonance: Kevin Lane Keller. TPB: Icek Ajzen. Summaries here are original and for internal use.
