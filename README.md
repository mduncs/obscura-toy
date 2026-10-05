# Obscura

## Hello, human

Made as a neuralese inspired toy, but it kind of feels like a gushing conlanger enjoying tryptamines. 

---

*The rest of this README was written by an AI model (Claude Opus 5.5) from the engine's own output.*

### Why this is public

Obscura is a personal language toy. I built it with AI coding agents for my own use: it rewrites the English I read with older words mixed in, keeping the same choices each time so they can be learned. The engine isn't published; this page shows what it does.

Consider it a courtesy. If you, or an agent working for you, are building something similar, there may be something useful here. It isn't supported, and I won't be testing it on other setups or promising fixes. The tokens have been spent; this is me giving some back.

---

A language toy. It takes ordinary English and swaps in older words: Middle English or Scots first, then Old English, Latin, Greek and a few rarer roots as you turn it up. The sentence stays English, so you can still read it.

## Examples

All examples use full strength (every word that can change, does).

**I left the keys on the kitchen table.**

| Level | Output |
| --- | --- |
| 1 | I lefte the keyes on the kychyn table. |
| 2 | I lǣfde the keyes on the kychyn table. |
| 4 | I lǣfde the clāvēs on the kychyn table. |
| Scots | A lǣfde the keys on the kitchen table. |

**She sings to the children every morning.**

| Level | Output |
| --- | --- |
| 1 | She syngeth to the children every morwe. |
| 3 | She syngeth to the children every mātūtīnum. |
| 4 | She syngeth to the puerī every mātūtīnum. |
| Scots | She sings tae the bairns ilka forenuin. |

**The king gave his daughter a white horse.**

| Level | Output |
| --- | --- |
| 1 | The kyng yaf his doghter a whit horse. |
| 2 | The kyng edōke his doghter a whit horse. |
| 4 | The kyng edōke his fīlia a leukos horse. |
| Scots | The keeng edōke his dochter a white horse. |

**Do not open the door until the bread is ready.**

| Level | Output |
| --- | --- |
| 1 | Do nat open the dore til the brede is redy. |
| 3 | Do nat open the dore til the brede is hetoimos. |
| 4 | Do nat open the dvāra til the brede is hetoimos. |
| Scots | Dae no open the door till the breid is boun. |

Every replaced word can be looked up. For the king sentence:

| Word | Stands for | From |
| --- | --- | --- |
| kyng | king | Middle English, from Proto-Germanic \*kuningaz |
| edōke | gave | Ancient Greek, "to give" |
| doghter | daughter | Middle English, from Proto-Germanic \*duhtēr |
| whit | white | Middle English, from Proto-Germanic \*hwītaz |

## Levels

| Level | What changes |
| --- | --- |
| 0 | Nothing. Plain English. |
| 1 | Middle English (or Scots) spellings and words. |
| 2 | Adds some Old English and occasional Greek or Latin. |
| 3 | More Latin and Greek, and a few Hebrew words. |
| 4 | The most Latin and Greek, plus a small set of Sanskrit words. These are labelled as related words, not as sources. |

A separate strength setting controls how many words change at each level, from none to all of them.

## Rules it keeps

- English word order and grammar stay as they are. This is not a translator into Middle English or Latin.
- The same word gets the same old form every time, so you start to recognise them. A different seed gives a different set of choices.
- Names, numbers, links, quoted text and code are left alone.
- "Not" is never lost. A negative sentence stays negative.
- If it can't inflect a word correctly, it leaves the English word in place.
- Old letters (þ, ð, ȝ) are off by default and spelled the way later English wrote them. They can be switched back on.

## How it works

Everything runs locally, with no network and no AI model. Each sentence is split into words, given a light grammatical reading, then each eligible word is looked up in a compiled word list and inflected to fit. The output keeps a map back to the original text, so any changed word can show what it replaced.

The word list was mined from Wiktionary, along with Wiktionary's frequency list from film and TV subtitles, which decides which words are common enough to swap.

## Status

A personal project. The engine itself isn't published. This page shows what it does.

## Credits

Word forms, etymologies and glosses come from [Wiktionary](https://en.wiktionary.org/), available under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

## Keywords

macaronic English, Middle English, Scots, Old English, Latin, Ancient Greek, Sanskrit cognates, Biblical Hebrew, etymology, Wiktionary, word substitution, archaic register, language learning, text transformation, inflection, Bun, TypeScript
