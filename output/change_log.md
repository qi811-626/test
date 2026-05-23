# Change Log: 管会pre_revised.pptx

Source file: `管会pre.pptx`  
Revised file: `output/管会pre_revised.pptx`  
Revision date: 28 May 2026

## Summary

- Revised the presentation using the workflow in `skills/pptx/SKILL.md`: content extraction, XML unpacking, direct text/notes editing, cleanup, repacking, and content QA.
- Preserved the original PowerPoint file and wrote the revised version to `output/管会pre_revised.pptx`.
- Replaced all incorrect speaker-note dates `1.7.2013` with `28 May 2026`.
- Updated the title slide date from `2026.05.28` to `28 May 2026`.
- Improved English phrasing throughout the deck to make the language more natural, concise, and suitable for a university classroom presentation.
- Standardised title capitalisation, punctuation, spacing, and label formatting.
- Condensed the Case Study slide by shortening the scenario, principle breaches, and outcomes.
- Rewrote speaker notes as oral presentation prompts instead of slide-reading scripts.
- Reformatted the references slide closer to APA 7 style by using corporate authors, year formatting, sentence-case titles, and direct URLs.

## Slide-Level Changes

| Slide | Main revisions |
| --- | --- |
| 1 | Updated title wording and date format. |
| 3 | Clarified the APES 110 overview and improved principle descriptions. |
| 4 | Improved application wording and removed duplicated wording. |
| 5 | Improved wording for confidentiality and professional behaviour. |
| 6 | Fixed label spacing and clarified application/exception language. |
| 7 | Compressed the case study and corrected awkward phrasing in outcomes. |
| 8 | Tightened conclusion language and made the final takeaway more formal. |
| 9 | Cleaned the references heading and revised references toward APA 7 style. |
| 10 | Simplified the closing slide to `Thank You` and `Questions?`. |

## Validation

- `pack.py` validation passed when rebuilding `output/管会pre_revised.pptx`.
- `markitdown` text extraction was run on the revised file to verify slide text and speaker notes.
- Searched the revised output for stale dates, placeholder text, malformed labels, and common encoding artifacts.
- Local visual rendering with `soffice`/`pdftoppm` could not be run in the Codex desktop environment because those executables were not available.
