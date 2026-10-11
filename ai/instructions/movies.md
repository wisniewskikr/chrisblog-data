Instructions:
* Category "Movies" is always about exactly one TED talk (https://www.ted.com/).
* The user prompt contains a "TED talk facts" block (link, title, speaker, description, topics) for the talk found from the hints. Treat its values as authoritative.
* In the hints, the line "<surname>; <talk title>" only identifies the talk. The text below it is the author's notes about the talk — the only source of the body content.
* Field "Title" must have the format "TED - <talk title>; <speaker full name>". English version: the exact talk title from the facts. Polish version: the Polish title (use the author's title from the hints if it is in Polish, otherwise translate). Never translate the speaker's name. Example: "TED - Jak zrobić ze stresu swojego przyjaciela; Kelly McGonigal" / "TED - How to make stress your friend; Kelly McGonigal".
* Field "Description" must be based on the Description from the facts: 1–5 sentences, plain text (no Markdown, no headings), at most 700 characters. Translate it into Polish for the Polish version. Do not add facts that are not in the TED description.
* If the "TED talk facts" block has no Description line, write the description from the author's notes instead (same rules: 1–5 sentences, plain text, at most 700 characters), without adding facts that are not in the notes.
* Field "Body (Markdown)" must have the format:
  # Content
  <bullet list>
  # TED
  You can watch the whole talk on [TED](<TED talk link>).
  Translate headings and sentences into Polish for the Polish version ("# Treść", "Cały wykład obejrzysz na [TED](<link>).").
* The bullet list is the author's notes rewritten as short bullet points ("less is more"): one idea per bullet, usually 3–8 bullets, repetitions merged, numbered points from the notes kept as a numbered list. It should read as a short educational text about the talk.
* Fix typos, grammar and the spelling of names and terms in the notes (e.g. "Oksytozen" -> "oksytocyna"). You may add a short, widely known clarification when a note is unclear, but do not invent studies, numbers, quotes or claims the talk does not make.
* Do not add a description, summary or cover image to the body — the blog shows the description and the cover image in a separate section above the body. Do not add any images to the body.
* If there is no "TED talk facts" block, do not guess: use "MISSING TED DATA" as the title and as the description in both languages.