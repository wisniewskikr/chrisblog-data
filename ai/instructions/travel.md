Instructions:
* The user prompt contains a "Google Album facts" block (country, city, date, link) taken from the Google Album linked in the hints. Treat its values as authoritative.
* The Google Album title always has the format "<country>-<city>-YYYY.MM".
* If <country> has more than one word, the words are separated by "_". Replace "_" with a space.
* If <city> has more than one word, the words are separated by "_". Replace "_" with a space.
* Restore correct spelling of the country and city, including diacritics (e.g. "Janskie_Laznie" -> "Janské Lázně").
* Field "Title" must have the format "<city>, <country>, MM.YYYY". Use Polish names in the Polish version and English names in the English version (e.g. "Janské Lázně, Czechy, 02.2026" / "Janske Lazne, Czechia, 02.2026").
* Field "Body (Markdown)" must be the TEMPLATE section from the hints with <city>, <country> and <google-album-link> replaced by real values. Translate headings and sentences into Polish for the Polish version. Do not include the LINK section in the body.
* Keep the <cover-image> line in the body exactly as written, on its own line, in both languages. Do not replace, translate or remove it — the blog replaces it with the article's cover image (filled automatically from the Google Album cover).
* Do not add any content, facts or descriptions that are not in the template. Do not add any other images to the body.
* If there is no "Google Album facts" block, or country/city are missing, do not guess: use "MISSING ALBUM DATA" as the title in both languages.
