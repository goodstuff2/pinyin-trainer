# Pinyin Trainer

A cartoon-style n-back game for learning Chinese pinyin. Each card shows a Chinese
word with its pinyin and definition; N cards later you spell that word's pinyin,
one letter at a time. Missed words come back a few cards later for extra practice.

Built from the 2000 Most Common Chinese Words in Context vocabulary list
(2000 words with pinyin and definitions, embedded in the page — works offline).

## Play

Open https://goodstuff2.github.io/pinyin-trainer/ — or download `index.html`
and open it in any browser (no server needed).

## How it works

- **N-back**: at N=2, when the 3rd card shows up, spell the 1st card's pinyin.
  Hit 80%+ to level up, drop below 60% to level down.
- **No timer** (default): the round only moves on after you answer, Enter to advance.
  Chill / Normal / Zippy timed modes optional.
- **One letter at a time**: each letter has its own box; a wrong letter ends the word
  as a miss and the correct spelling is revealed.
- **Spaced review**: a missed word returns 3–5 cards later.
- Definition shown beside each new word; the answered word parks on the right
  for review.
- Round length: 10 + 8×N scored words. Progress is saved in localStorage.
