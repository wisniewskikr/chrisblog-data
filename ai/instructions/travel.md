Instructions:
* The user prompt contains a "Google Album facts" block (country, city, date, link) taken from the Google Album linked in the hints. Treat its values as authoritative.
* The Google Album title always has the format "<country>-<city>-YYYY.MM".
* If <country> has more than one word, the words are separated by "_". Replace "_" with a space.
* If <city> has more than one word, the words are separated by "_". Replace "_" with a space.
* Restore correct spelling of the country and city, including diacritics (e.g. "Janskie_Laznie" -> "Janské Lázně").
* Field "Title" must have the format "<city>, <country>, MM.YYYY". Use Polish names in the Polish version and English names in the English version (e.g. "Janské Lázně, Czechy, 02.2026" / "Janske Lazne, Czechia, 02.2026").
* Field "Description" must be exactly this sentence with <city> and <country> replaced by real values, as plain text (no Markdown, no headings): "The article describes a trip to <city> in <country>." Translate it into Polish for the Polish version.
* Field "Body (Markdown)" must be exactly the text below with <google-album-link> replaced by the link from the "Google Album facts" block. Translate the heading and the sentence into Polish for the Polish version.
  # Google Album

  Pictures from this area you can find in my [Google Album](<google-album-link>).
* Do not add a description, summary or cover image to the body — the blog shows the description and the cover image in a separate section above the body.
* Do not add any content or facts that are not described in these instructions. Do not add any images to the body.
* If there is no "Google Album facts" block, or country/city are missing, do not guess: use "MISSING ALBUM DATA" as the title and as the description in both languages.
