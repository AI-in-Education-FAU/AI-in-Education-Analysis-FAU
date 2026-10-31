# AI in Education | FAU

**Exploring how artificial intelligence in education is discussed, understood, and experienced in public discourse.**

[**Explore the Research Workbench**](https://warm-mousse-9e6c33.netlify.app/) · [**GitHub Organization**](https://github.com/AI-in-Education-FAU)

## About the Project

Artificial intelligence is reshaping conversations about teaching, learning, assessment, and the future of education. These conversations take place not only in academic research and institutional policy, but also in news coverage and public comment sections, where people share their expectations, concerns, and experiences.

**AI in Education | FAU** is a research initiative focused on studying that public conversation. The project brings together tools for collecting publicly accessible news articles and comments and analyzing their language with natural language processing (NLP) methods. Our goal is to support systematic, transparent, and reproducible investigation of how AI in education is represented and debated across online sources.

Rather than treating a single model's output as definitive, the research workflow supports comparing methods, checking results against human judgments, and reviewing uncertain or conflicting classifications.

## What We're Exploring

The project is designed to help researchers investigate questions such as:

- **Public sentiment:** How positively, negatively, or neutrally do people discuss AI in education?
- **Perspectives and disagreement:** Which positions do commenters take on AI-related claims, and how do they respond to one another?
- **Emerging themes:** What topics and concerns appear most often in news coverage and public discussion?
- **Stakeholder voices:** How do different groups describe the opportunities and challenges associated with educational AI?
- **Emotions and framing:** What reactions accompany discussions of AI-enabled teaching, learning, and assessment?
- **Research reliability:** How do different NLP approaches compare, and when is human review needed?

These are research questions the platform helps investigate, not conclusions that the tools assume in advance.

## An End-to-End Research Workflow

The initiative connects two complementary tools into a research workflow:

### 1. Discover and collect public discourse

The **[News Article & Comment Collector](https://github.com/AI-in-Education-FAU/News-Aggregator-Articles-and-Comments-Collector)** helps researchers find and gather publicly accessible articles and their associated comments. Its active, user-facing sources are **Yahoo News** and **MSN**.

Researchers can discover articles using keywords, collect from selected URLs, extract article text and metadata, and capture available public comments and reply threads. They can inspect collected data, export it in structured formats, and prepare or upload records to a shared **Supabase** database.

This component creates the evidence base for subsequent analysis. It is a separate desktop application, not a feature of the web workbench.

### 2. Explore, analyze, and validate the data

The **[Text Analysis Workbench](https://github.com/AI-in-Education-FAU/text-analysis-workbench)** provides a browser-based research environment for exploring articles and comments stored in Supabase.

Researchers can organize work into projects, filter and inspect texts, and run multiple NLP approaches over selected material. Supported research tasks include:

| Research task | What it helps examine |
| --- | --- |
| **Sentiment analysis** | Positive, negative, and other sentiment classifications in text |
| **Stance analysis** | Agreement, disagreement, and positions toward claims or parent comments |
| **Topic modeling** | Recurring subjects, themes, and patterns across texts |
| **Stakeholder classification** | Potential stakeholder perspectives or self-identifications |
| **Emotion analysis** | Emotional signals expressed in public discourse |
| **Custom codebooks** | Researcher-defined categories relevant to a particular study |

The workbench supports complementary methods, including rule-based and lexicon approaches, topic models, transformer-based models, and optional large language model analyses. Researchers can compare outputs, flag disagreement or low confidence, evaluate against human reference labels, and approve, correct, reject, or exclude results. Findings and associated classifications can then be exported for further research.

**[Open the Research Workbench →](https://warm-mousse-9e6c33.netlify.app/)**

## How the Pieces Fit Together

```text
Public news articles and comments
          │
          ▼
  News Article & Comment Collector
  Discover · Extract · Inspect
          │
          ▼
    Structured research data
       (CSV / JSON / Supabase)
          │
          ▼
     Text Analysis Workbench
   Explore · Analyze · Compare
          │
          ▼
    Human review & validation
          │
          ▼
   Exportable research results
```

**The collector and the workbench are distinct applications.** The collector supports data acquisition and preparation; the workbench supports interpretation, methodological comparison, and review. Supabase provides the shared data layer when records are uploaded and made available to the workbench.

## Research Principles

Our approach emphasizes:

- **Transparent methodology.** Analysis methods and saved runs can be inspected and compared rather than accepted as black-box answers.
- **Human oversight.** Automated classifications can be checked against reference labels and reviewed or corrected by researchers.
- **Reproducibility.** Structured datasets, saved analyses, and exportable outputs support repeatable research workflows.
- **Responsible data collection.** The collection tool is intended for publicly accessible content and does not bypass authentication, paywalls, or CAPTCHAs.
- **Careful interpretation.** Online news comments are not representative of every educator, student, or community; automated labels can be uncertain or biased and require contextual interpretation.

## Project Repositories

| Repository | Purpose |
| --- | --- |
| [News-Aggregator-Articles-and-Comments-Collector](https://github.com/AI-in-Education-FAU/News-Aggregator-Articles-and-Comments-Collector) | Desktop tool for discovering and collecting publicly accessible news articles and comments, with structured exports and Supabase integration. |
| [text-analysis-workbench](https://github.com/AI-in-Education-FAU/text-analysis-workbench) | Web application for project-based text exploration, NLP analysis, method comparison, human validation, and research exports. |
| [AI-in-Education-Analysis-FAU](https://github.com/AI-in-Education-FAU/AI-in-Education-Analysis-FAU) | General research-platform overview repository. |

For installation, configuration, testing, and deployment instructions, see the README and documentation in the relevant repository.

## Who This Is For

The project is intended for researchers and collaborators studying **AI in education**, **public opinion**, **digital discourse**, and **computational social science**. Although the collection and analysis tools are motivated by education-related questions, the underlying workflow can also support other topics where publicly available text is studied systematically.

## Explore

**[Visit the Text Analysis Workbench](https://warm-mousse-9e6c33.netlify.app/)**  
**[Browse our GitHub repositories](https://github.com/AI-in-Education-FAU)**

---

*AI in Education | FAU — turning public conversations into researchable evidence through responsible data collection, computational analysis, and human interpretation.*
