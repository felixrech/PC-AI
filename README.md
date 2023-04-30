# PC-AI Dataset

The Public Consultation on the AI Act proposal (PC-AI) dataset contains the results of the [2021 public consultation](https://ec.europa.eu/info/law/better-regulation/have-your-say/initiatives/12527-Artificial-intelligence-ethical-and-legal-requirements/feedback_en?p_id=24212003) on the [draft of the Artificial Intelligence Act (AI Act)](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:52021PC0206). The feedback received (`feedbacks.csv`) and their attachments (`attachments.csv`, `attachments/`) have been scraped from the 'Have your Say' platform using our library [hys_scraper](https://github.com/FelixRech/hys_scraper/).

Though they can be computed from the overall feedbacks, some summary statistics (`categories.csv`, `countries.csv`)have also been scraped. The text of each PDF attachment has been extracted using [PyMuPDF](https://pypi.org/project/PyMuPDF/) and is available as a text file in the `attachments/` folder.

## Patches

Additionally, we also offer a patched version (`patched_feedback.csv`) making the following changes - see `patch_script.ipynb` for details:

- Reclassify several feedbacks from the `other` user type into their proper user types
- Fix a typo in the 'Have your Say' API (i.e. rename user type `academic_research_instittution` [sic.])
- Remove some accidental submissions and the same feedback submitted multiple times by the same person

## White paper

The [public consultation on the original AI white paper](https://ec.europa.eu/info/law/better-regulation/have-your-say/initiatives/12527-Artificial-intelligence-ethical-and-legal-requirements/public-consultation_en) is also available in the [white_paper branch](https://github.com/felixrech/PC-AI/tree/white_paper).
