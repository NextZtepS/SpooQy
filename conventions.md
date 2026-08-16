# SpooQy Obsidian Vault — Conventions & Structure

> **Purpose**: This file is a skill reference for any LLM assistant helping to maintain and grow this Obsidian vault. Read this file first before creating, editing, or linking any notes.

---

## 1. Vault Overview

This is an academic research vault for the **SpooQy quantum optics lab**. It is organized around three core directories that form a clean separation of concerns:

| Directory | Role | Contains |
|---|---|---|
| `Notes/` or root | **Ideas & concepts** | Topic notes, derivations, explanations |
| `Sources/` | **Bibliographic index** | One `.md` per paper — the canonical linking point |
| `Originals/` | **Raw files** | PDFs organized in topic sub-folders |

> Notes may live either in the `Notes/` folder or directly in the vault root. Both are valid.

---

## 2. Directory Structure

```
SpooQy/
├── conventions.md
├── <TopicNote>.md
├── Notes/
│   └── <TopicNote>.md
├── Sources/
│   └── <Topic>/
│       └── <Author YYYY>.md
├── Originals/
│   └── <Topic>/
│       └── <YYYY - Author - Full Title>.pdf
└── .obsidian/
```

---

## 3. Sources File Convention

Every paper referenced in the vault **must** have a corresponding file in `Sources/`.

### 3.1 Naming

```
Sources/<Topic>/<First Author Lastname> <YYYY>.md
```

Where `<Topic>` is the exact folder name used in `Originals/` (e.g. `SPDC`, `Quantum Internet`, `Quantum Dots`, `EOM`).

For papers with many authors, use `et al.`:
```
Sources/Steinlechner et al. 2014.md
```

### 3.2 Template

```markdown
---
Authors:
  - "[[Firstname Lastname]]"
  - "[[Firstname Lastname]]"
Publication: "[[Journal Name]]"
Title: Full paper title here
Year: "YYYY"
tags:
  - TopicTag
---
[[YYYY Full paper title as it appears in Originals.pdf|Full paper title here]]
```

### 3.3 Rules

- **Authors**: Each author is a `[[wikilink]]` so that author pages can be created and linked in the graph.
- **Publication**: The journal or conference is also a `[[wikilink]]`.
- **Year**: Stored as a `text` string (quoted), not a number — per `types.json` config.
- **Tags**: Use the topic sub-folder name from `Originals/` as the tag (e.g., `SPDC`).
- **Body**: A single wikilink to the PDF file in `Originals/`, using a pipe `|` alias for the human-readable title. The PDF filename must match exactly.

### 3.4 Example

```markdown
---
Authors:
  - "[[Alexander Lohrmann]]"
  - "[[Chithrabhanu Perumangatt]]"
  - "[[Aitor Villar]]"
  - "[[Alexander Ling]]"
Publication: "[[Applied Physics Letters]]"
Title: Broadband pumped polarization entangled photon-pair source in a linear beam displacement interferometer
Year: "2019"
tags:
  - SPDC
---
[[2019 Broadband pumped polarization entangled photon-pair source in a linear beam displacement interferometer.pdf|Broadband pumped polarization entangled photon-pair source in a linear beam displacement interferometer]]
```

---

## 4. Originals File Convention

PDFs are stored in `Originals/<Topic>/` where `<Topic>` matches the tag used in Sources.

### 4.1 Naming

```
Originals/<Topic>/YYYY - <Author> - <Full paper title>.pdf
```

Where `<Author>` follows this rule:
- **≤ 5 authors**: use the first author's last name only (e.g., `Lohrmann`)
- **> 5 authors**: use first author's last name followed by `et al.` (e.g., `Steinlechner et al.`)

Examples:
```
Originals/SPDC/2014 - Steinlechner et al. - Efficient heralding of polarization-entangled photons from type 0 and type II SPDC in PPKTP.pdf
Originals/SPDC/2019 - Lohrmann - Broadband pumped polarization entangled photon-pair source in a linear beam displacement interferometer.pdf
Originals/SPDC/2021 - Anwar - Entangled photon-pair sources based on three-wave mixing in bulk crystals.pdf
```

### 4.2 Rules

- Year comes **first** in the filename, enabling chronological sorting.
- Follow the `YYYY - Author - Title` format with ` - ` (space-dash-space) as the separator.
- Author field: first author's last name only if ≤ 5 authors; first author's last name + `et al.` if > 5 authors.
- Use the **full title** (no truncation) to make the wikilink self-documenting.
- The filename in the `Sources/` wikilink must **exactly match** the actual PDF filename.

---

## 5. Topic Note Convention

Topic notes explain concepts, summarize fields, and link out to sources and other concepts.

### 5.1 Naming

Use the concept name directly as the filename:
```
SPDC.md
ppKTP crystal.md
bipartite entanglement.md
```

### 5.2 Structure

```markdown
#ConceptName

## Definition

> [!note] Definition
> Short, precise definition of the concept. Use [[wikilinks]] to related concepts inline.

## <Section>

Prose explanation. Cite sources using [[Author YYYY]] wikilinks.
Deep-link to specific PDF pages for precise claims.

## <Section>

...
```

### 5.3 Obsidian Markdown Features Used

#### Callouts (Admonitions)
Used for definitions, warnings, key results:
```markdown
> [!note] Title
> Content here.

> [!warning] Title
> Content here.

> [!tip] Title
> Content here.
```

#### LaTeX Math
Inline and block math is supported:
```markdown
Inline: $\ket{H} \rightarrow \ket{HH}$
Block:
$$
\ket{\Phi^+} = \frac{1}{\sqrt{2}}(\ket{HH} + \ket{VV})
$$
```

#### Wikilinks — Three Patterns

| Pattern | Syntax | Use case |
|---|---|---|
| Link to a Source | `[[Lohrmann 2019]]` | Cite a paper |
| Link to a concept Note | `[[ppKTP crystal]]` | Reference another topic |
| Deep-link to PDF page (page only) | `[[filename.pdf#page=N\|label]]` | LLM-safe citation |
| Deep-link to PDF page + selection | `[[filename.pdf#page=N&selection=S,s,E,e\|label]]` | Precise in-text citation (human-generated) |

#### PDF Deep-Link Syntax

There are two variants of PDF deep-links:

**Variant A — Page-only (LLM-safe, always use this when writing programmatically):**
```markdown
[[2014 Efficient heralding...pdf#page=2|page 2]]
```

**Variant B — Page + text selection (human-generated only):**
```markdown
[[2014 Efficient heralding...pdf#page=2&selection=151,41,194,10|page 2]]
```

| Fragment | Meaning | Source |
|---|---|---|
| `page=N` | Page number in the PDF | Can be determined by reading the PDF |
| `selection=S1,L1,S2,L2` | Character offset indices of the highlighted text | **Computed by Obsidian's PDF.js renderer only** |
| `\|label` | Display text shown in the note | Descriptive label e.g. `page 2` |

> **LLM Convention**: An LLM reading a PDF (e.g., via `pdftotext`) can reliably determine page numbers but **cannot compute `selection=` coordinates**. These offsets are internal character positions calculated by Obsidian's embedded PDF viewer when a user highlights text and right-clicks → *"Copy link to selection"*. They do not correspond to character positions in the plain-text extraction.
>
> **Rule**: LLMs must always write `#page=N` links only. If `&selection=...` is needed for precision, the human adds it afterward in Obsidian by highlighting the relevant passage and replacing the bare page link.

---

## 6. The Linking Chain

The standard citation flow is:

```
Topic Note
  └─ [[Author YYYY]]
        └─ Sources/Topic/Author YYYY.md    (has frontmatter metadata)
              └─ [[YYYY Title.pdf|Title]]
                    └─ Originals/Topic/YYYY Title.pdf
```

For precise in-text citations, a Note may also **directly deep-link** to a PDF page, bypassing Sources:
```
Topic Note
  └─ [[YYYY Title.pdf#page=N|page N]]
        └─ Originals/Topic/YYYY Title.pdf  (opens at page N)
```

Both patterns can coexist in the same sentence:
```markdown
...as shown in [[Steinlechner et al. 2014]] [[2014 Efficient heralding...pdf#page=2&selection=151,41,194,10|page 2]].
```

---

## 7. Frontmatter Property Types

Defined in `.obsidian/types.json`. Do not deviate from these types:

| Property | Type | Notes |
|---|---|---|
| `Authors` | `multitext` | List of `"[[wikilink]]"` strings |
| `Publication` | `multitext` | Single `"[[wikilink]]"` string |
| `Title` | `text` | Plain string, no wikilink |
| `Year` | `text` | Quoted string e.g. `"2019"` |
| `tags` | `tags` | Unquoted list items. **No spaces allowed** — use CamelCase for multi-word topics (e.g., `QuantumInternet` not `Quantum Internet`) |

---

## 8. Installed Plugins

| Plugin | Purpose |
|---|---|
| `editing-toolbar` | Community plugin — rich-text formatting toolbar in the editor |

---

## 9. Quick Reference Checklist

When **adding a new paper**:
- [ ] Place PDF in `Originals/<Topic>/YYYY - Author - Full Title.pdf` (≤5 authors: lastname only; >5 authors: lastname + `et al.`)
- [ ] Create `Sources/<Topic>/<Author YYYY>.md` with full frontmatter (topic subfolder must match the `Originals/` subfolder)
- [ ] Ensure the wikilink in the Sources body **exactly matches** the PDF filename
- [ ] Tag the Sources file with the topic folder name
- [ ] Add `[[Author YYYY]]` citations in relevant topic Notes

When **creating a new topic Note**:
- [ ] Use `#ConceptName` as the H1 heading (no space after `#`)
- [ ] Use `> [!note]` callout for definitions
- [ ] Wrap concept names in `[[wikilinks]]` even if the note doesn't exist yet (ghost links are fine — they encourage future note creation)
- [ ] Cite papers using `[[Author YYYY]]` and optionally add a PDF deep-link immediately after

When **creating a new topic folder** in `Originals/`:
- [ ] Use a short, capitalized topic name (e.g., `SPDC`, `Entanglement`, `Tomography`)
- [ ] Multi-word folder names must be written in **CamelCase** as the tag (e.g., folder `Quantum Internet` → tag `QuantumInternet`) — Obsidian does not support spaces in tags
- [ ] Use that exact CamelCase tag value in all Sources files for papers in that folder
