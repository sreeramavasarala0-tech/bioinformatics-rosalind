# AI Usage Log (Module 03)

## 1) Gemini (Google AI Studio)
**What I asked for:** Examples to practice assignment operator, data types, and a quick Biopython installation test snippet.  
**Prompt snippets:**
- "Give me 3 tiny Python examples that demonstrate the assignment operator `=` clearly."
- "Write a one-cell Biopython installation check for Colab that imports `Bio` and prints the version."

**What I changed before committing:**
- Rewrote variable names to follow lower_snake_case.
- Added exception handling so the notebook doesn’t crash if `Bio` isn’t installed.
- Inserted comments to match course style.

**How I verified correctness:**
- Ran cells in a fresh Colab runtime; confirmed `pip` install message and version.
- Executed code without errors; ensured outputs match expectations.

## 2) ChatGPT (OpenAI)
**What I asked for:** Clean, lecture-aligned notebook outline covering `print`, `input`, lists/slicing, conditionals, loops, file I/O, dictionaries, and Biopython (`Seq`, `SeqIO`, `gc_fraction`).  
**Prompt snippets:**
- "Draft a Colab-ready notebook scaffold that mirrors our week-3 topics with clear, runnable cells and minimal dependencies."
- "Add robust `input()` handling and file I/O demonstrations using `read`, `readline`, `readlines`, and `join`."

**What I changed before committing:**
- Adjusted messages and variable examples to fit our class vocabulary.
- Ensured robust defaults (e.g., created small example FASTA files inside the notebook).

**How I verified correctness:**
- Ran all cells top-to-bottom locally and in Colab.- Spot-checked Biopython outputs (complement, reverse_complement, transcribe, translate).


## 3) DeepSeek
**What I asked for:** A compact function pair for (a) transcribing an input FASTA to RNA and (b) reporting the record with max GC%.  
**Prompt snippets:**
- "Write two Python functions: `transcribe_fasta_to_rna(in_fasta, out_fasta)` using Biopython, and `max_gc_record(in_fasta)` returning (best_id, gc%). Keep it dependency-light."

**What I changed before committing:**
- Added explicit imports inside functions to keep them portable.
- Appended `_RNA` to output IDs to avoid collisions and clarify provenance.
- Added rounding and clear return formats.

**How I verified correctness:**
- Created a small test FASTA inline, ran both functions, inspected outputs.
- Cross-checked GC% values with manual `count()` based spot checks.

