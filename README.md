# Responsible LLM Project Guide

An interactive, seven-step guide from **Google DeepMind: AI Research Foundations** for planning a language-model project with real-world impact, built around ethical, community-centred practice. Each step opens in a zoomed view with tasks, response boxes, side notes and links to further resources.

## How it works

- **Progress map:** a winding path of seven steps. Click a step to zoom in, and mark each one *Not started*, *On going* or *Completed*.
- **Tasks and response boxes:** every task has one or more text fields for your own answers, with word counts where the course sets a length (for example 150–200 words for the problem statement, 250–300 for the governance brief).
- **Side notes:** each task carries short notes (see below) that point you to values, frameworks, examples and resources.
- **Data Card:** the answers you write in Step 2 build up into a Data Card that you can copy out as Markdown.
- **Saved in your browser:** responses and progress are stored in localStorage, so nothing is sent to a server. Clearing site data resets the guide.

## The seven steps

| # | Step | Time | What you produce |
| --- | --- | --- | --- |
| 1 | **Develop your problem statement** | 30 min | Your values, candidate problems, an evaluation of them, and a 150–200 word problem statement |
| 2 | **Build a dataset ethically with a Data Card** | 60 min | A draft Data Card covering inputs and outputs, classification, labelling, data creation, web collection ethics, bias and representation, and values alignment |
| 3 | **Create an impact statement card** | not specified | Who is affected, intended and unintended impacts, how you will measure them, and a card-sized impact statement |
| 4 | **Design a mini-engagement plan** | 45 min | Two stakeholder groups, their priorities, harms and benefits, and an engagement method for each |
| 5 | **Design a governance blueprint for your LLM** | 60 min | Benefits and risks, a governance action for each, and a 250–300 word governance brief |
| 6 | **Design a sustainability plan for your LLM project** | 60 min | Actions at developer, stakeholder and organisational level, and who decides and is responsible |
| 7 | **Best practices for sharing your work** | 10 min | A cleaned-up notebook, a style guide, a Git repository, a README and a licence |

Step 3's tasks are a suggested structure, because the original course instructions for it weren't available. The page says so in a notice. Check them against the course page.

## Side notes

Notes appear next to tasks and are colour-coded by kind:

| Kind | What it gives you |
| --- | --- |
| **Tip** | Practical advice for the task, such as scoring ideas against values or having two people label the same sample |
| **Did you know?** | Short real-world context, such as RobotsMali, the AlphaFold database and the EU AI Act |
| **From your sources** | Ideas drawn from the course readings, such as data colonialism, the "algorithmic imprint" and relational ethics |
| **Ubuntu value** | Interconnectedness, Communal Character and Moral Motivation, each with guidance on when to apply it |
| **Governance proposal** | "Fair Tech" Ecosystem (inspired by Fair Trade) and Data Trusts and Cooperatives (data stewardship) |
| **Licences to check** | MIT, Apache 2.0 and Creative Commons, and when each fits |

Some tasks also have checklists and prompts: *A good problem statement should…*, *Sentence starters*, *Your Data Card should record*, *Frameworks to cite*, *Governance approaches for inspiration*, and *A README typically includes*.

## Resources linked in the guide

**Step 1: Problem statement**
- [AlphaFold Protein Structure Database](https://alphafold.ebi.ac.uk/), an example of research with real-world impact

**Step 2: Data Card**
- [Data Cards Playbook](https://sites.research.google/datacardsplaybook/), for Sections 1–3 (Explore, Define, Create)
- [World Bank Open Data](https://data.worldbank.org/)
- [Awesome Public Datasets](https://github.com/awesomedata/awesome-public-datasets)
- [Hugging Face Datasets](https://huggingface.co/datasets)
- [Google Dataset Search](https://datasetsearch.research.google.com/)
- [Kaggle Datasets](https://www.kaggle.com/datasets)
- [CARE Principles for Indigenous Data Governance](https://www.gida-global.org/care) (Global Indigenous Data Alliance)

**Step 4: Engagement plan**
- [Action Catalogue](https://actioncatalogue.eu/), for methods such as Participatory Design, User Committees, Deliberative Workshops and Distributed Dialogue

**Step 6: Sustainability**
- [CodeCarbon](https://codecarbon.io/), which tracks emissions from your training code
- [ML CO2 Impact calculator](https://mlco2.github.io/impact/), which estimates emissions by hardware and region

**Step 7: Sharing your work**
- [Google Python Style Guide](https://google.github.io/styleguide/pyguide.html)
- [PEP 8](https://peps.python.org/pep-0008/)
- [GitHub](https://github.com/)

## Cited reference

Pushkarna, M., Zaldivar, A. and Kjartansson, O. 2022. *Data Cards: Purposeful and Transparent Dataset Documentation for Responsible AI.* FAccT '22: 2022 ACM Conference on Fairness, Accountability and Transparency, Seoul.

## Run locally

The page is a single self-contained file with no build step. Because it re-reads its own source at runtime, open it through a local web server rather than by double-clicking the file:

```bash
python -m http.server 8000
# then visit http://localhost:8000
```

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The guide (content, styles and runtime in one file) |
| `support.js` | Standalone copy of the runtime that is already inlined in `index.html`; not referenced by the page |
| `LICENSE` | License terms |

## External dependencies

Loaded from CDNs at view time, so an internet connection is needed:

- Google Fonts (Cormorant Garamond, Outfit, DM Sans, JetBrains Mono)
- Remix Icon (jsDelivr)
- Iconify flat-color icons

## License

See [LICENSE](LICENSE).
