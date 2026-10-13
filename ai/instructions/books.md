Instructions:
* Category "Books" is always about exactly one book. The user prompt contains a "Book facts" block (link, title, author, original title, publisher, year, description). Treat its values as authoritative.
* In the hints, the line "<surname>; <title>" under BOOK DETAILS only identifies the book. The text under BOOK CONTENT is the author's notes — the only source of the body content.
* Field "Title" must have the format "<full book title>; <author full name>". Polish version: the full Polish title from the facts. English version: the original title from the facts if it is in English, otherwise a translation of the Polish title. Use normal capitalization, not the capitals from the hints. Never translate the author's name. Example: "Jak nakarmić świat. Historia i przyszłość żywności; Vaclav Smil".
* Field "Description" must be based on the Description from the facts: 1–5 sentences, plain text (no Markdown, no headings), at most 700 characters. Translate it into English for the English version. Do not add facts that are not in the book description.
* The notes are split into sections by lines made only of two or more "-" characters. Process each section separately and keep their order. The first line of a section (e.g. "WSTĘP", "1. CO ZAWDZIĘCZAMY ROLNICTWU?") becomes a "##" heading in normal capitalization, with its numbering kept. Do not output the separator lines.
* Each section's notes become short bullet points ("less is more"): one idea per bullet, repetitions merged, checkbox markers such as "[  ]" removed.
* Fix typos, grammar and the spelling of names and terms in the notes (e.g. "Marnotrastwo" -> "Marnotrawstwo", "sporzywać" -> "spożywać"). You may add a short, widely known clarification when a note is unclear, but never change facts or numbers and never invent studies, numbers or quotes.
* Field "Body (Markdown)" must have the format:
  # Content
  ## <section heading>
  <bullet list>
  (one "##" block per section)
  # Link
  Link to the book: [<book title>](<Book link>)
  Translate headings and sentences into Polish for the Polish version ("# Treść", "# Link", "Link do książki: [<tytuł>](<link>)").
* Do not add a description, summary or cover image to the body — the blog shows the description and the cover image in a separate section above the body. Do not add any images to the body.
* If there is no "Book facts" block, do not guess: use "MISSING BOOK DATA" as the title and as the description in both languages.