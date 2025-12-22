---
layout: about
title: About
permalink: /
subtitle: <b>Workshop at the Conference on Neural Information Processing Systems (NeurIPS) 2025</b>

profile:
  align: right
  image: berts.png
  image_circular: false # crops the image to make it circular
  more_info: 

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

The NeurIPS workshop on *Recent Advances on Time Series Foundation Models: Have We Reached the BERT Moment?* will be held at the San Diego Convention Center on December 7, 2025.
A hackathon will be organized shortly after the workshop to foster the development of benchmarks and applications where TSFMs can truly shine. Details will be provided in time. We look forward to welcoming you to San Diego. 

**Location**: San Diego Convention Center, Upper Level Room 3<br>
**Date**: Sunday 7<sup>th</sup> December 2025

### Social Mixer (sponsored by The Forecasting Company)

We are excited to announce a social mixer for all workshop participants, generously sponsored by [The Forecasting Company](https://www.theforecastingcompany.com/en). The event will take place on Sunday, December 7th, from 5:30 PM to 8:30 PM, immediately following the workshop sessions. This mixer will provide an excellent opportunity for attendees to network, share ideas, and discuss the latest advancements in time series foundation models in a relaxed and informal setting. We look forward to seeing you there for an evening of engaging conversations and connections!

You can register for the workshop and social event [here](https://luma.com/wnqz9wix).

### Introduction

Foundation models (FMs) have achieved great success in NLP and vision, inspiring over 20 new time series FMs (TSFMs) in the past year. Despite promising results, studies show that carefully designed lightweight supervised baselines often match TSFM performance. Unlike NLP's "BERT Moment," TSFMs still require full fine-tuning to be competitive in real-world scenarios. Additionally, some tabular FMs rival TSFMs without being time series-specific. Recent benchmarks also provide mixed evidence: GIFT-Eval favors TSFMs, OpenTS shows statistical models outperforming deep learning on univariate data, and FoundTS finds supervised baselines on par with TSFMs. This workshop aims to bring together researchers to examine the gap between TSFM potential and real-world utility, and to identify benchmarks and applications where TSFMs can truly excel.

The key topics of this workshop include, but are not limited to:
- Benchmarking Foundation Models in Time Series,
- Scaling Laws and Efficiency in Time Series Models,
- Evaluating Transferability and Adaptability of Foundation Models,
- Leveraging Foundation Models of Other Modalities for Time Series,
- Unsupervised performance estimation of TSFMs,
- Industrial Benchmarking of Time Series Foundation Models

More details are provided in our [Call for Papers](/call-for-papers/).

### Accepted papers
The full list of accepted papers can be found [here](/accepted-papers/).
The following papers were selected for an oral presentation.
- **Efficiently Generating Correlated Sample Paths from Multi-step Time Series Foundation Models** -- Ethan Baron, Boris N. Oreshkin, Ruijun Ma, Hanyu Zhang, Kari Torkkola, Michael W. Mahoney, Andrew Gordon Wilson, Tatiana Konstantinova
- **Pre-trained Forecasting Models: Strong Zero-Shot Feature Extractors for Time Series Classification** -- Andreas Auer, Daniel Klotz, Sebastian Böck, Sepp Hochreiter
- **FlowState: Sampling-Rate Invariant Time Series Foundation Model with Dynamic Forecasting Horizons** -- Lars Graf, Thomas Ortner, Stanisław Woźniak, Angeliki Pantazi
- **CHRONOGRAPH: A Real-World Graph-Based Multivariate Time Series Dataset** -- Luțu Adrian-Cătălin, Ioana Pintilie, Andrei Manolache, Elena Burceanu

### Schedule
**Sunday 7th December 2025, Upper Level Room 3, San Diego Convention Center** <br>
This is a tentative schedule subject to change. Please take a look at the [NeurIPS website](https://neurips.cc/) for the detailed schedule.

| **Time (PST)**                                | **Event**                                                                                                                                                                   |
|:------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 8:30 - 08:45                  | 🥁 **Welcome and introduction**                                                                                                                                              |
| 8:45 - 9:15                  | 📢 **Invited Talk by <a href="https://www.cs.cmu.edu/~atalwalk/">Ameet Talwalkar</a>** <br /> <small>Vertical AI Meets Observability<small/>                                                                                       |
| 9:20 - 9:50                 | 📢 **Invited Talk by <a href="https://sites.google.com/view/liuchenghao/home">Chenghao Liu</a>** <br /> <small>[From Time Series Foundation Model to Reasoning and Agentic Systems: A Roadmap for Emergent Anomaly Detection Intelligence](/assets/pdf/chenghao_slides.pdf) <small/>                                                                           |
| 9:50 - 10:05                 | ☕ **Coffee & Networking Break**                                                                                                             |
| 10:10 - 10:25                 | 🎤 **Contributed Spotlight Talk - <a href="https://www.linkedin.com/in/tatiana-konstantinova">Tatiana Konstantinova</a>** <br /> <small>[Efficiently Generating Correlated Sample Paths from Multi-step Time Series Foundation Models](/assets/pdf/Konstantinova.pdf)<small/>                                                                                           |
| 10:25 - 10:40                 | 🎤 **Contributed Spotlight Talk - <a href="https://apointa.github.io/">Andreas Auer </a>** <br /> <small>[Pre-trained Forecasting Models: Strong Zero-Shot Feature Extractors for Time Series Classification](/assets/pdf/Zero-Shot-Classification-Slides.pdf)<small/>                                                                                                          |
| 10:40 - 11:40                 | 📑 **Poster Session 1**                                                                                                                                   |
| 11:45 - 12:45                 | 🦞 **Lunch Break**   |
| 12:50 - 13:20                 | 📢 **Invited Talk by <a href="https://dcmaddix.github.io/">Danielle M. Robinson</a>** <br /> <small>[Understanding the Bitter Lesson in Time Series Foundation Models](/assets/pdf/robinson_slides.pdf)<small/>                                                                             |
| 13:25 - 13:55                 | 📢 **Invited Talk by <a href="https://www.ml.informatik.tu-darmstadt.de/people/mkraus/index.html">Maurice Kraus</a>** <br /> <small>[Do We Really Need Another Time-Series Forecasting Model?](/assets/pdf/kraus_slides.pdf)<small/>                                         |
| 13:55 - 14:10                 | ☕ **Coffee & Networking Break**                                                                                                                           |
| 14:10 - 15:00                 | 🎓 **Pannel Discussion (<a href="https://www.aiml.informatik.tu-darmstadt.de/people/fdivo/">Felix Divo</a>, <a href="https://sites.google.com/view/liuchenghao/home">Chenghao Liu</a>, <a href="https://sites.google.com/site/qingsongwen8/">Qingsong Wen</a>, <a href="https://www.cs.cmu.edu/~atalwalk/">Ameet Talwalkar</a>)**                                                                                                                                                             |
| 15:00 - 15:15                 | ☕ **Coffee & Networking Break**                                                                                                                           |
| 15:15 - 15:30                 | 🎤 **Contributed Spotlight Talk by <a href="https://www.linkedin.com/in/lars-graf-a0008b296/">Lars Graf</a>** <br /> <small>FlowState: Sampling-Rate Invariant Time Series Foundation Model with Dynamic Forecasting Horizons<small/>                                                                                                                              |
| 15:30 - 15:45                 | 🎤 **Contributed Spotlight Talk by <a href="https://www.linkedin.com/in/lutu-adrian-7a1b8526b/">Luțu Adrian-Cătălin</a>** <br/> <small>[CHRONOGRAPH: A Real-World Graph-Based Multivariate Time Series Dataset](/asset/pdf/ChronoGraph.pdf)<small/>                                                                   |
| 15:45 - 16:45                 | 📑 **Poster Session 2**                                                                                  |
| 16:45 - 17:00                 | 🎬 **Concluding Remarks & Hackaton Ad**                                          |
| 17:30 - 20:30                 | 🍻 **Social Event**                                          |
{: .table}
{: .table-striped}

### Contact
If you have questions, you can contact [Thomas Moreau](mailto:thomas.moreau@inria.fr) and [Ievgen Redko](mailto:ievgen.redko@gmail.com) or send an email to [berts2025.workshop@gmail.com](mailto:berts2025.workshop@gmail.com).

### Sponsors
  <a href="https://www.theforecastingcompany.com/en/" target="_blank">
      <img src="/assets/img/TFC_LOGO_original.png" alt="The Forecasting Company" width="200">
  </a>   
  <a href="https://sig.com/" target="_blank">
      <img src="/assets/img/susquehanna_logo.png" alt="Susquehanna" width="200">
  </a>

We thank [The Forecasting Company](https://www.theforecastingcompany.com/en) for generously supporting the organization of the social event for the participants of the workshop (more details to come soon) an  [Susquehanna](https://sig.com/) for sponsoring the Best Paper Award. 

