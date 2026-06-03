# lexlog — what it is and why I'm building it

Working name: lexlog. A personal, experimental app. Built for my daily reading, not for an audience. Everything below is about my own experience.

## The pain

I started reading recently — books, blogs, newsletters, the occasional short story. I hit unfamiliar words constantly.

My current loop is simple: see a word I don't know, search it in Perplexity, read the meaning. If it's tricky, I paste the whole sentence so I understand how it fits. Then I move on.

The lookup itself works fine. That's not the problem.

The problem is what happens next: nothing. The word goes nowhere.

Days later I hit the same word in another book, and I've forgotten it. So I look it up again — same word, same sentence-pasting, same effort. I've "learned" some words three or four times and still don't own them.

The real gap is that the moment of curiosity gets thrown away every time. I do the work of understanding a word and then have no way to meet it again on purpose. I only re-encounter words by accident, which is slow and repetitive — I'm relearning instead of remembering.

So the app isn't a better dictionary. It's the thing that catches the word after I understand it and makes sure I see it again — without me having to plan a study session, because I won't.

## How it works, end to end

I open the app. I'm already on the input — no dashboard, no menu.

I type the word, optionally paste the sentence I found it in, and tap explain. I get a plain meaning and, if I gave a sentence, an explanation of how the word fits that exact moment.

If I want more — an example, whether it's formal or casual, where it came from — I just keep asking. Same as Perplexity, but focused only on the word.

When I'm satisfied, I save it. That's the one thing Perplexity never did: it kept the word.

After that I do nothing.

A widget on my home screen shows me a saved word and the sentence it came from. I glance at it in the gaps I already have — unlocking my phone, waiting for something. I tap the word to test whether I remember the meaning, then reveal it.

"Got it" moves me on and counts toward mastering it. "Still learning" skips it back into the queue with no penalty. A word becomes mine only after I've recalled it correctly enough times across different days.

## Why each piece earns its place

I'm only keeping features that fix the actual pain. Here's what each one does for me specifically.

### The lookup saves the word

This is the whole point. I already do the lookup; now the work doesn't evaporate. Every word I was curious enough to check ends up somewhere instead of being thrown away. I stop relearning words I've already understood once.

### I can keep asking follow-ups

A single definition often isn't enough for a word to stick — I understand it better when I see a second example or learn it's a formal word I'd never say out loud. Letting me ask follow-ups means I explore until the word actually lands, instead of half-getting it and moving on. Keeping it scoped to just the word stops it from becoming a general chatbot I get lost in.

### The sentence comes with the word

I remember words by where I met them, not as dictionary entries. Saving the original sentence means when the word resurfaces later, it shows up with the context that made it click the first time. That sentence is the memory hook.

### The widget does the remembering for me

I will not open a flashcard app every day. I know this about myself. The widget removes the need to — the word finds me in moments I'm already spending on my phone. No session to start, no habit to build. This is the feature that actually closes the loop between looking a word up and owning it.

### Tap-to-reveal forces a one-second recall

Just reading a word again doesn't make it stick — I'd recognize it without being able to use it. Hiding the meaning until I tap makes me try to recall first. That one second of effort is the difference between recognizing a word and knowing it.

### Mastery is by confirmation, not by schedule

I didn't want a system that tells me I'm "behind" or breaks a streak. Words move forward only when I genuinely recall them, and failing one never resets my progress — it just brings the word back sooner. A word leaves the rotation when I've proven it's mine, not when a calendar says so. No pressure, no guilt, which means I'll actually keep using it.

### My Words is a searchable record

Sometimes I half-remember a word — I recall the sentence but not the word, or the other way around. The list lets me search across the word, the meaning, and the sentence, so I can find it from whatever fragment I've got. It's also just satisfying to see the collection grow.

### On-device, offline, private

I read in places with bad signal, and I don't want a lookup to fail mid-book or cost anything. Running the model on the phone means it always works, costs nothing per word, and my reading stays on my device. For an app I'm building only for myself, that's the right trade.

## What's deliberately out (for now)

Kept minimal on purpose, because anything I won't use is clutter:

- No quiz or scroll mode inside the app — the widget handles review.
- No dungeon screen yet — mastered words just stay in the list.
- No tags, decks, folders, or settings beyond the basics.
- No sharing from the browser or other apps yet — manual input only.
- No sync — local storage first.
- No streaks, no gamification, no notifications pestering me.

These aren't rejected ideas, just things that don't earn their place in the first version. The bar is simple: does it fix the lookup-and-forget loop? If not, it waits.

## The one line

I look a word up, understand it, and the app makes sure I meet it again — on my home screen, in the gaps I already have — until it's mine. No studying required, because I know I won't.
