# Startfleet-Academy-
Starfleet Academy repo. Dictation education from Spock's Vulcan learning — rapid, immersive, application-first. Building explorers who turn science fiction into a Starfaring civilization


![Banner](./assets/banner.png)

> Starfleet Academy repo. Dictation education from Spock's Vulcan learning — rapid, immersive, application-first. Building explorers who turn science fiction into a Starfaring civilization.

## What this is

Starfleet Academy is a co-pilot for learning by speaking. A question is asked, you predict out loud, and the gap between that prediction and the source is closed immediately. What gets kept is your own restatement of the closed gap, not a transcript.

![How the loop feels](./assets/loop.png)

## Quick start

Paste this to Copilot to jumpstart a build:

```text
You are the Starfleet Academy co-pilot. Build the smallest loop that does this:

1. Speak one question from the learner's current source.
2. Wait for a spoken prediction. Do not explain first.
3. Compare that prediction to the local source on this computer.
4. Close only the gap, then ask the learner to restate it in their own words.
5. Save that restatement into their Obsidian vault. Do not save a transcript.

Read the config in this file and personalize the loop to that learner. Keep it rapid, and keep learning next to application.
```

## A personalized academy

One learner, one config. Fill this in and the co-pilot should follow it.

```yaml
learner:
  name: ""
  prerequisites: []
vault:
  path: ""                 # Obsidian vault on this computer
  note_rule: "closed-gap restatement only"
voice:
  input: "whisper"         # or an open voice model
sources:
  truth: "local"           # files on this computer
  lenses: []               # chosen sources, not a textbook sequence
loop:
  order: ["question", "prediction", "gap", "restatement"]
  pace: "rapid"
```

## Values

Learning is the shrinking gap between a prediction and the source's explanation. The prediction comes first, and it will be wrong. That wrong move is the point.

The workflow is one person at a time. When you are stuck, say the idea out loud. Retrieval is dictation, then a check against source truth that lives on your computer, so the match is not a generic one.

The loop is rapid on purpose. Question, answer, correction, restatement. AI is there to close the gap, not to replace the restatement. Obsidian holds the result: local-first, and only the articulation of a gap you have already closed.

## Links

- [Documentation](https://example.com/docs)
- [Repository](https://example.com/repo)
- [Issues](https://example.com/issues)

Replace the example links, and drop real images at `assets/banner.png` and `assets/loop.png`.
