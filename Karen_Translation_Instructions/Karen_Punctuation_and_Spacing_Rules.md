# S'gaw Karen Punctuation and Spacing Rules (with fix-up steps)

**Standard used:** the edited Karen text of *The Ministry of Healing*, chapters 1–4 (MH_Karen_Edit_1.0.txt, lines 1–267). These four chapters are clean and consistent. They contain 896 commas, 845 full stops and 103 quotations. The rules below describe what they do.
**Checked against:** the rest of MH (chapters 5–22), DA1-16.txt (Desire of Ages), and Karen STC Draft (tagged).txt (Steps to Christ).

---

## Part A. The rules

### 1. Characters (use standard Unicode, not old-font characters)
The clean text uses only standard Unicode S'gaw Karen. Some files still contain characters from older fonts. Replace them as follows:

| Wrong (old font) | Correct | Example |
|---|---|---|
| ၥ (U+1065) | ာ (U+102C) | ခရံၥ် → ခရံာ် |
| ၁် (digit one + ်) | ာ် | လၢ၁် → လၢာ် |
| ၀ (digit zero) **inside a word** | ဝ (letter WA, U+101D) | အ၀ဲ → အဝဲ |
| ၦ (U+1066) | ပှ | ၦၤကညီ → ပှၤကညီ |
| ၇ှ (digit seven + ှ) | ၡ | ယ၇ှါယၤ → ယၡါယၤ |
| ရှ (letter ra + ှ) | ၡ | ယ့ၣ်ရှူး → ယ့ၣ်ၡူး, ယရှါယၤ → ယၡါယၤ (chapters 5–22 of MH, about 200 times) |
| ၇ (digit seven) before a vowel sign inside a word | ရ | ခ၇ံ၁် → ခရံာ် |
| ႇ (U+1087, Shan tone mark used as a comma) | , | လုၢ်ဟံၣ်ႇ တၢ် → လုၢ်ဟံၣ်, တၢ် |

The opposite mistake also happens. **Inside a number, use the digit ၀, not the letter ဝ.** For example, write ၁၀ and ၃၀, not ၁ဝ and ၃ဝ. MH has 17 of these, including in chapter 1: မၢ်ကူး ၁:၃ဝ.

### 2. Punctuation marks
1. **Use the Western comma and full stop `,` `.`** Never use the Burmese ၊ or ။.
2. **Every sentence ends with a final particle and then a full stop.** The particle depends on the kind of sentence:

| Sentence type | Ending |
|---|---|
| statement | …လီၤ. |
| negative (တ … ဘၣ်) | …ဘၣ်. |
| "why / how / who / what" question | …လဲၣ်. |
| yes/no question | …ဧါ. |
| command, request, invitation | …တက့ၢ်. |
| completed action, often in quoted verses | …လံ. |

3. **Do not use `?` or `!`.** An English question or exclamation still ends with a full stop in Karen. The particle shows that it is a question or exclamation.
   - ✘ `ဒ်လဲၣ်?` → ✔ `ဒ်လဲၣ်.`
   - ✘ `ဂ့ၤဒိၣ်!` → ✔ `ဂ့ၤဒိၣ်လီၤ.`
4. **Use curly double quotes `“ ”`.** Do not use straight quotes `"` or single quotes `' '`. A quotation inside a quotation also uses `“ ”`, because the clean text has no single quotes at all.
5. **The full stop or comma goes inside the closing quote.** Write `…လီၤ.”` and `…စံးဝဲ,”`. Never write `”.` or `”,` (the clean text has 85 of `.”` and none of `”.`).
6. **Introduce a quotation with a comma.** Write `…စံးဘၣ်အီၤ, “…”`.
7. **An English dash (—) becomes a hyphen with no spaces around it.**
   - `စံးဆၢအမိၢ်-ဒီးတၢ်စံးဆၢ…`
   - `မၤဘျါပှၤဆူးပှၤဆါ-တၢ်လၤကပီၤ…`
8. **Write an ellipsis as spaced full stops: `. . .`** after a full sentence, the stop plus three dots: `…လီၤ. . . ဒီး…`. Replace `…`, `...` and `....` with this form.
9. **Use commas where the Karen needs them.** This is much more often than in English. The clean text uses them:
   - before **ဒီး** ("and") when it joins clauses or the items of a list;
   - after each item in a "whether … or …" list: `X မ့ၢ်ဂ့ၤ, Y မ့ၢ်ဂ့ၤ,`;
   - after a time or condition clause (ending in **အခါ**, or starting with **ဖဲ …**, **မ့ၢ် …** or **လၢ … အဂီၢ်**);
   - before a quotation (rule 6).

### 3. Spacing
1. **No spaces between Karen words.** A sentence runs together until the next punctuation mark. Word breaks are made later with zero-width spaces (rule 6 below), not with normal spaces.
2. **Exactly one space after every comma and full stop.** The exceptions are: at the end of a line, and before a closing quote.
   - ✘ `လီၤ.တၢ်` → ✔ `လီၤ. တၢ်`
3. **No space before a comma, a full stop or a closing quote.**
4. **Never use two spaces in a row, and don't leave spaces at the end of a line.**
5. **These normal spaces are allowed:**
   - after punctuation;
   - between a Bible book name and its numbers (`မးသဲ ၈:၁၇`);
   - between a book number and the book name (`၁ ကရံၣ်သူး`);
   - after a comma between verse numbers (`၂:၄၈, ၄၉`);
   - before the `{MH …}` tag;
   - in headings such as `အဆၢဒိၣ် ၁`.
6. **Zero-width spaces (ZWSP) come last.** Add them with a script, following section 3 of *Karen Translation_Instructions*. Do this only after all the other fixes, so that the ZWSP rule sees correct text.

### 4. Numbers and Bible references
1. **Use Karen numerals (၀–၉) for Bible references, chapter numbers and numbers in the text.** Keep the Arabic numerals inside the Ellen White tags: `{MH 17.1}`.
2. **Write a reference as: book name, one space, chapter:verse.** Use a comma and space between verses and a hyphen for a range.
   - `လူၤကၣ် ၂:၄၈, ၄၉`
   - `ယိၤဟၣ် ၄:၇-၁၄`
   - "Verses 29, 39" becomes `အဆၢဖိ ၂၉, ၃၉`.
3. **For a numbered book, put a space after the number:** `၁ ကရံၣ်သူး ၁၃:၄`, `၂ မိၤၡ့ ၃၃:၁၈`. Not `၂မိၤ`.
4. **When the English puts a reference after a quotation, the Karen does the same.** Write the reference after the closing quote, followed by a full stop:
   - `…လီၤ.” မးသဲ ၈:၁၇.`
5. **A reference on its own (with no quoted words) goes in parentheses,** as section 4 of the instruction file says:
   - `(မၢ်ကူး ၅:၂၃)`

### 5. Headings, tags and layout
1. **Chapter heading:** `အဆၢဒိၣ် ၁` on its own line, using Karen numerals. Put nothing after the number: no `း`, no full stop, no English such as "Chap. 12" or "MH, Chap. 17". The chapter title goes on the next line.
2. **Section headings and titles have no final punctuation.**
3. **Each paragraph ends with its tag, after one space:** `…လီၤ. {MH 17.1}`. **Tag format (decided):** `{` + book code + space + page.paragraph + `}`, with **no space after `{`** or before `}`. This applies to every book (`{MH 17.1}`, `{SC 9.1}`, `{DA 19.1}`), even when the English source has `{ MH 17.1}`. Keep the Arabic numerals.
4. **Leave one blank line between paragraphs.** Drop the English page numbers. Join any paragraph that was split across a page break back into one line.
5. **Poetry or verse that is split over several lines in the English becomes one paragraph in Karen,** with commas between the lines.
6. **A chapter ends with a line containing only `#`.**

---

## Part B. Order of work when fixing a file

Do the steps in this order. Each step depends on the one before.

1. **Separate the Karen from the English.** This is needed only where the two are on the same line, as in MH chapters 12–22, which use the layout `English {MH tag} <tab> Karen`. Keep the tag with the Karen paragraph.
2. **Convert old-font characters** (Part A, section 1). Do this before anything else, because ႇ is really a comma and ၀ is really a letter. Afterwards, fix ဝ inside numbers back to the digit ၀.
3. **Fix the punctuation marks** (section 2):
   - straight quotes to curly quotes;
   - `?` and `!` to the correct particle and a full stop;
   - all ellipsis forms to `. . .`;
   - `”.` to `.”`.
4. **Fix the spacing** (section 3):
   - remove spaces between Karen letters;
   - add the missing space after `,` and `.`;
   - remove the space before punctuation;
   - collapse double spaces and remove spaces at the end of lines.
5. **Fix references, headings and tags** (sections 4 and 5).
6. **Read through by hand.** Removing a stray space can join two words that were really two sentences with the full stop missing, so check those places.
7. **Add the ZWSPs with the script.**

### Searches for checking a finished file (regular expressions)
| Problem | Search for | Should find |
|---|---|---|
| space between Karen words | `(?<=[က-႟]) (?=[က-႟])` | only between a book name and its numbers, or in headings |
| missing space after punctuation | `[,.](?=[က-႟“])` | nothing |
| space before punctuation | ` [,.”]` | only inside `. . .` |
| old-font characters | `[ၥၦႇ]\|၁်\|၇[ှံ]\|ရှ` | nothing |
| digit zero inside a word | `(?<![၀-၉])၀(?![၀-၉])` | nothing |
| letter WA inside a number | `[၀-၉]ဝ\|ဝ[၀-၉]` | nothing |
| wrong quotes or marks | `["'?!…၊။]` | nothing (in the Karen) |
| punctuation outside the quote | `”[.,]` | nothing |
| double or end-of-line spaces | `  \| +$` | nothing |
| space inside a tag | `\{ \| \}` | nothing |

---

## Part C. What each project needs

| File / part | State | Main fixes needed |
|---|---|---|
| **MH chapters 1–4** | The standard | Very little. 7 numbers use letter ဝ (e.g. ၁:၃ဝ). There are a few double spaces and missing blank lines between paragraphs. One `?` (ch. 2, `…ဖိ?လၢ…`). Two opening quotes are the wrong way round (`”လံာ်` in MH 21.1, and `”ဒီး` once elsewhere). |
| **MH chapters 5–11** | Old-font text | 1,672 ၥ to convert, and 1,731 ၀ that should be the letter ဝ. 4,693 spaces between words. 343 straight quotes. 8 `?`/`!`. 3 `…`. Headings have `း` (၇း, ၈း, ၁၀း, ၁၁း). There are no {MH} tags; these need adding from the English. |
| **MH chapters 12–22** | English and Karen on the same line, old font | Split the English and Karen first (306 lines, plus 186 English-only lines such as poems). Then convert 294 ၥ, 219 ၦ, 585 ႇ (comma), 141 ၁်, about 26 ၇, and 299 ၀. Remove 2,452 spaces between words. Fix 66 straight quotes and mixed ellipsis forms. Headings read "Chap. 12" / "MH, Chap. 17" / "Chapter 20" and need cleaning up. Chapters 13–16 have no heading of their own that the scan could find, so check them by hand. |
| **DA1-16.txt** (Desire of Ages) | Unicode is fine | 2,549 spaces between words. 186 straight quotes. Ellipsis written `....`. Numbered book written `(၂မိၤ …)` should be `(၂ မိၤ …)`. The chapter headings are `(၁)`, `(၂)`; change them to `အဆၢဒိၣ် ၁` if you want them to match MH. There are no Ellen White tags. |
| **Karen STC Draft (tagged).txt** (Steps to Christ) | Nearly finished, already has ZWSPs | 5 `!` to change. 11 `…` to change to `. . .`. 422 spaces between words (see Decision 2). One `”.` (Tags were corrected to `{SC …}` on 11 Oct 2026.) |

---

## Part D. Decisions for you
1. **Tag format — decided:** use `{MH 17.1}`, with no space after `{`, for all books (see rule 5.3). The English source files (MH, Steps to Christ ×2, Desire of Ages) and the three Karen STC drafts were corrected to this form on 11 Oct 2026, so copying the English tag exactly now gives the right result. Note that section 3 of *Karen Translation_Instructions* still says to copy the tag exactly as the English has it. That still works now that the English tags are fixed.
2. **Phrase spaces.** The STC draft keeps some normal spaces between phrases (for example `တၢ်ဘၣ်တ့ ဒီး လံာ်စီဆှံ`), as many printed Karen books do. The edited MH text has removed them all. These rules follow MH (no spaces), so confirm that's what you want before the spaces are removed from STC and DA.
3. **Quotation followed by a reference.** MH writes `…လီၤ.” မးသဲ ၈:၁၇.` (no brackets), but STC writes `…လီၤ.” (ယိၤဟၣ် ၁:၁၈)`. These rules follow the English layout of each book. If you'd rather always use brackets, change rule 4.4.
4. **Dash.** The clean text uses a plain hyphen for the English dash. An en dash (–) would look more like the English but isn't used anywhere yet.
