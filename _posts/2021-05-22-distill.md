---
layout: distill
title: a distill-style blog post
description: an example of a distill-style blog post and main elements
tags: distill formatting
giscus_comments: true
date: 2021-05-22
featured: true
mermaid:
  enabled: true
  zoomable: true
code_diff: true
map: true
chart:
  chartjs: true
  echarts: true
  vega_lite: true
tikzjax: true
typograms: true

authors:
  - name: Albert Einstein
    url: "https://en.wikipedia.org/wiki/Albert_Einstein"
    affiliations:
      name: IAS, Princeton
  - name: Boris Podolsky
    url: "https://en.wikipedia.org/wiki/Boris_Podolsky"
    affiliations:
      name: IAS, Princeton
  - name: Nathan Rosen
    url: "https://en.wikipedia.org/wiki/Nathan_Rosen"
    affiliations:
      name: IAS, Princeton

bibliography: 2018-12-22-distill.bib

# Optionally, you can add a table of contents to your post.
# NOTES:
#   - make sure that TOC names match the actual section names
#     for hyperlinks within the post to work correctly.
#   - we may want to automate TOC generation in the future using
#     jekyll-toc plugin (https://github.com/toshimaru/jekyll-toc).
toc:
  - name: Equations
    # if a section has subsections, you can add them as follows:
    # subsections:
    #   - name: Example Child Subsection 1
    #   - name: Example Child Subsection 2
  - name: Citations
  - name: Footnotes
  - name: Code Blocks
  - name: Interactive Plots
  - name: Mermaid
  - name: Diff2Html
  - name: Leaflet
  - name: Chartjs, Echarts and Vega-Lite
  - name: TikZ
  - name: Typograms
  - name: Layouts
  - name: Other Typography?

# Below is an example of injecting additional post-specific styles.
# If you use this post as a template, delete this _styles block.
_styles: >
  .fake-img {
    background: #bbb;
    border: 1px solid rgba(0, 0, 0, 0.1);
    box-shadow: 0 0px 4px rgba(0, 0, 0, 0.1);
    margin-bottom: 12px;
  }
  .fake-img p {
    font-family: monospace;
    color: white;
    text-align: left;
    margin: 12px 0;
    text-align: center;
    font-size: 16px;
  }
---

At NeurIPS 2025, we organized the workshop "Recent Advances in Time Series Foundation Models" to address a pivotal question: while NLP and Computer Vision have been transformed by foundation models, why does the Time Series (TS) community often feel like it is playing catch-up?

To explore this, we held a panel discussion chaired by [Thomas Moreau](https://tommoral.github.io), featuring insights from [Ameet Talwalkar](https://www.cs.cmu.edu/~atalwalk/), [Felix Divo](https://www.aiml.informatik.tu-darmstadt.de/people/fdivo), [Chenghao Liu](https://sites.google.com/view/liuchenghao/home), and [Qingsong Wen](https://sites.google.com/site/qingsongwen8/). The conversation spanned the technical hurdles of tokenization, the debate over "universal" models, and the future of benchmarking. Below are some of the key takeaways from the session.

This discussion showed that there is a strong need to improve the benchmarking methodology for TSFM, and we propose to host a **benchmark creation sprint in Paris on the 28th and 29th of May**. More details in the [conclusion](#conclusion-a-call-to-action).

### 1. Why are we "late to the game"?

The session opened by addressing the elephant in the room: Why haven't Time Series Foundation Models (TSFMs) seen the same explosive adoption as models in other modalities?
Ameet pointed out a **historical resource disparity**, as efforts and compute have overwhelmingly favored image and text, due to general public interest. However, Felix offered a more technical reason: for decades, **simple baselines were surprisingly sufficient** for TS tasks. Unlike in NLP, where deep learning offered an immediate, massive leap over N-grams, TS statistical methods held their ground for a long time.

Chenghao and Qingsong highlighted a structural challenge: **fragmentation**. "Time series" isn't a single domain; it covers finance, healthcare, weather, and speech. As audience members noted, these sub-communities often operate in silos, like speech or brain signal processing, making it difficult to unify them under one architectural roof.

### 2. Generalization vs. Specificity: Can one model do it all?

A major debate emerged regarding the feasibility of a single "General" Time Series model.

Chenghao warned against blindly mixing datasets, noting that key information varies drastically between tasks (e.g., the signal in music vs. the signal in stock prices). A significant hurdle raised by the audience is non-stationarity, particularly in finance where adversarial factors create complex causal graphs that don't exist in physical systems like weather.
Thomas synthesized this challenge by noting that a universal model needs to cope with the "*different ranges of regularity*" across these domains -- some signals are highly predictable and regular, while others are chaotic, making a unified model architecture difficult to tune.

Ameet suggested that to bridge this gap, we need **multimodality**. Since TS data often lacks context (missing information), feeding the model exogenous variables—like text or video—can help it "understand" the system better than raw numerical values alone.

### 3. Moving beyond forecasting (and the MAE trap)

The panel reached a consensus that the community focuses too heavily on forecasting and leaderboard metrics like Mean Absolute Error (MAE). Chenghao argued that forecasting is rarely the end goal. It is usually an intermediate step towards a decision (e.g., buying a stock, treating a patient). Therefore, minimizing MAE doesn't always correlate with downstream success. However, forecasting is a compeling task as it does not require labelling to evaluate.

Felix added that for TSFMs to be truly useful, they must demonstrate capabilities beyond prediction. The "foundation model" promise is versatility—handling imputation, anomaly detection, and classification with the same backbone, a challenge often overlooked by the community.

### 4. What are the next steps for the community?

To move the field forward and achieve a true "BERT moment," the panel identified three priorities:

- **The "Usability" Moment:** Felix argued that we need a "ChatGPT moment"—not just in terms of performance, but accessibility. Models must be easy for end-users to adapt to new tasks without massive re-engineering.
- **Trustworthy Benchmarking:** Ameet emphasized that while we have more benchmarks than ever, the ecosystem is scattered. We need a trusted, common ground for evaluation to know which models actually work in real-world scenarios.
- **Causality:** Qingsong identified causal reasoning as the critical next frontier. Understanding why a series behaves the way it does is essential for robustness.

### Conclusion: A Call to Action

The most critical takeaway from the discussion is the urgent need for a unified, high-quality evaluation framework. While Time Series Foundation Models have shown promise, their true impact cannot be measured until we standardize how we assess their performance across diverse applications.

We, the organizers, are responding to this call by hosting a **benchmark creation sprint in Paris on the 28th and 29th of May**.
The goal of this sprint is to leverage the `benchopt` framework to create a single, diverse benchmark. This will aim to unify evaluation across disparate datasets (like gift-eval, fev, and boom) and critical tasks (forecasting, classification, and anomaly detection) to foster a less scattered, more collaborative ecosystem.
If you are intersted in participating, **please fill in [this form](https://docs.google.com/forms/d/e/1FAIpQLSdTAl-KskFMXC_qXQFC0txJdyOGvHK4eymFF9DUYm5iNpef0w/viewform)**, so we can organize the logisitic.
Let' all come together to help the Time Series community achieve its foundation model breakthrough!
