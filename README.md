# lexlog — MVP

The product definition for the first build: scope, screens, and behaviour. It covers the product surface, not the technical decisions.

## Scope

The MVP does one thing end to end: I look up a word, save it, and the app resurfaces it until it's mine.

Everything in this build serves that loop. Anything that doesn't is left out.

## Platform and constraints

- Android only.
- Manual word input only — no browser capture, no share sheet.
- Local storage only — words live on the device, no account, no sync.
- On-device model — lookups run on the phone, offline, with no per-word cost.

These constraints define the MVP. They keep the first build small enough to finish and simple enough to use day to day.

## The three screens

### 1. Home — capture

Where I land when I open the app. The input is the screen — no dashboard, no menu.

- Books icon, top left → opens My Words.
- "lexlog", centered.
- A single input card: word field (large), sentence field below it (optional), explain button.
- Explain stays disabled until I type a word.

The home screen exists to get me from "I have a word" to "I understand it" in as few taps as possible.

### 2. Word exploration — conversation

Opens after I tap explain. This replaces the Perplexity step, but it keeps the word.

- Back arrow, top left → returns home and clears the input.
- The word is pinned in the header. If I gave a sentence, it sits below in small italic.
- Save button, top right — always visible, tappable at any point.
- The explanation appears first: plain meaning, plus how the word fits my sentence if I gave one.
- Three starter chips after the first reply: an example, formal or casual, origin.
- A follow-up field at the bottom for anything else about the word.
- Saving confirms briefly and returns me home.

The conversation is scoped strictly to the word — meaning, usage, register, origin, related words. It's not a general chatbot. Keeping it narrow is what makes it fast to use.

### 3. My Words

Reached from the books icon on Home. A plain record of everything I've saved.

- Back arrow, top left → returns home.
- A search field that matches across the word, the meaning, and the sentence.
- A list of entries: word, meaning, and the sentence if I saved one.
- Sorted by most recent first.

This screen is for finding a word again when I half-remember it — the sentence but not the word, or the reverse. Search across all three fields covers whichever fragment I've kept.

## The widget — review

The widget is the review surface. It handles review so I don't have to open the app and study, which I wouldn't do on my own.

- It shows one saved word and the sentence it came from.
- The meaning is hidden. I tap the word to test my recall, then reveal it.
- Two actions: "got it" and "still learning".
- "Got it" counts toward mastering the word and moves to the next one.
- "Still learning" changes nothing about my progress and moves to the next one.
- A word's count can only go up once per day, so I can't rush it.
- Words appear oldest-unmastered first.

For the MVP the widget advances only when I act on it — tap got it or still learning. Automatic rotation (on a timer, or on unlock) waits for later.

The sentence stays visible throughout. It's the memory hook — I remember a word by where I met it, not as a definition.

## Mastery

A word leaves rotation when I've recalled it enough times, not on a fixed schedule. The count climbs only when I confirm I know it, and never resets when I don't.

- 0–2 confirmations — fresh. Appears most often.
- 3–6 — familiar. Appears less.
- 7–14 — known. Appears rarely, as a reminder.
- 15 — mine. Effectively retired from the widget.

In this build a mastered word simply stays in My Words; there's no separate place for it to go. The thresholds still matter because they control how often the widget shows a word.

No streaks, no "you're behind", no penalty for forgetting. Pressure would make me stop using it.

## What a saved word holds

Each entry stores only what the loop needs:

- The word.
- Its plain meaning.
- The sentence I found it in, if I gave one.
- A confirmation count.
- When it was added.

The exploratory follow-ups aren't saved — they help the word land in the moment, but the entry stays minimal.

## Out of MVP

Not in the first build:

- Quiz or scroll review inside the app — the widget covers review.
- A dungeon screen for mastered words — they stay in the list for now.
- Browser and share-sheet capture — manual input only.
- Sync across devices — local first.
- Widget extras: meta row, source label, progress dots, automatic rotation.
- Tags, decks, folders, settings, streaks, notifications.

The test for adding any of these back: does it serve the look-up, save, resurface loop?
