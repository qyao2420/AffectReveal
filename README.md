# AffectReveal: Event-Grounded Emotion Recognition Beyond Visual Appearances

**Authors:** Yihao Qian, Runhao Zeng, Sicheng Zhao, Feng Liang, Hongmin
Cai, Mingkui Tan\
**Paper:** [arXiv:2609.36563](https://arxiv.org/pdf/2609.36563)\
**Dataset:** [EGER-Bench (Google
Drive)](https://drive.google.com/drive/folders/1QuWEC74H6n-gOUJWFWpjrSqhMLc9CIOu?usp=drive_link)

## Abstract

Visual emotion recognition commonly assumes that all evidence required
for prediction is contained in the observed image or video. Yet the same
visible reaction can convey different emotions depending on events
beyond the input: tears, for example, may indicate grief or joy. We
formulate **Event-Grounded Emotion Recognition (EGER)**, where emotion
recognition requires recovering the affect-determining event. We
construct **EGER-Bench**, comprising 10,052 videos and 10,734 images
across 11 emotions, two source domains, and four visual settings. A
study with six annotators shows that event context raises human
recognition accuracy from 33.96% to 72.08%, confirming that visual
evidence alone is often insufficient. Semantic relevance alone does not
solve EGER: a plausible event may imply the wrong emotion if its
identity, focal-person role, relationship, or outcome is misinterpreted.
We therefore propose **AffectReveal**, a tuning-free framework that
first constructs and independently verifies evidence-grounded
alternatives over these affect-critical factors. It then cross-checks
the recovered event against face-masked in-media facts through
bidirectional atomic evidence support, while retaining the original
unmasked input for final prediction. Across three downstream models and
four input settings, AffectReveal yields average UAR gains of
5.26--10.53 points. For three fine-tunable models, it also enables
untuned models to outperform their fine-tuned visual-only counterparts
in all 12 accuracy comparisons, without updating downstream parameters.

## Overview

### EGER-Bench

![EGER-Bench dataset
overview](https://arxiv.org/html/2609.36563v1/EGER-Bench_v5.png)

### AffectReveal

![AffectReveal framework
overview](https://arxiv.org/html/2609.36563v1/overview_v3.png)

------------------------------------------------------------------------

*The implementation code is not included in this repository at this
stage.*
