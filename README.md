# left-conspiracy

Investigative project on left-leaning conspiracy theories across Reddit
and other platforms.

## Repo structure

```
.
├── LOG.md              # shared research log — read this first
├── shared              # shared utilities, make sure are importable anywhere
├── notebooks/          # personal scratchspace - add everyone else's to gitignore, no need to pr if you push to branch and have changes here
│   └── sodi/
│   └── arushi/
│   └── nefriana/
├── raw/                #we gotta be careful here, not sure best approach for bigger files
├── docs/               # anything formal, again read section on LOG.md first
```


## The log

Try to always keep `LOG.md` updated, so each time you push code try to put a description.

The whole file is designed to paste into an LLM so everyone can be updated without reading through. Append-only;
don't edit prior entries, write new ones referencing them. Negative results are valued — write those up too. 

Suggested format is like: 
## 2026-04-24 — sodi — r/conspiracy 2023 topic exploration [exp:01]


**Did:** Pulled r/conspiracy submissions from the 2023 Reddit archive.
Computed sentence embeddings on title + selftext, ran PCA for
dim-reduction, generated wordcloud over the corpus.

**Found:** [fill in — top wordcloud terms, whether PCA components
looked interpretable, any obvious themes]. Coarse but useful as a
sanity check that the pipeline runs end-to-end and that conspiracy
register is recognizable in the output.

**Next:** Single-sub + single-year is too narrow for the comparative
left/right goal. Expand to a multi-sub, multi-year pull. 

**Files:** `notebooks/sodi/ex_s_01_first_reddit_pull`, outputs in same dir.