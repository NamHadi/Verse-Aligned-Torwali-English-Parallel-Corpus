Torwali-English verse-aligned corpus (Quranic part)
====================================================
Format: plain UTF-8, LF line endings, exactly ONE verse per LINE, no blank lines.
Line n of *.trw, *.en and *.ids is the same verse (ids = surah:verse).

full/ids.txt, full/trw.txt, full/en.txt   all 6,236 verses in Quranic order
full/corpus.tsv                           id <TAB> Torwali <TAB> English
full/ar_source_unchecked.txt              Arabic verses (pivot/source only; see note)
train.{ids,trw,en}                        5,436 verses, 94 surahs
dev.{ids,trw,en}                            402 verses, 11 surahs (15,24,59,63,70,72,75,78,83,97,100)
test.{ids,trw,en}                           398 verses,  9 surahs (25,28,31,43,46,48,58,64,114)
surah_split.tsv                           surah -> split

Split: by surah (no surah appears in two splits), random seed 2026, surahs of 5-100 verses
eligible for dev/test. Verse 1:1 is the basmala (as in Al-Fatiha); other basmala headers omitted.
English: Sahih International, leading "N. " numbering removed.
Torwali: NFC-normalized; whitespace collapsed.
Note: the Arabic text in some verses of Surah 33 (e.g. 33:45, 33:66-67) lacks spaces in the
source document; the Arabic file is not part of the Torwali-English pairs.
