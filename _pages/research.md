---
permalink: /research/
title: "Research"
---

I'm currently working with Dr. Erica Graham to understand the impact of hormonal fluctuations on lesion growth in endometriosis. This model is the first incorporating hormonal and receptor-binding dynamics in disease onset.

## Motivation

Endometriosis is a gynecological condition that presents with symptoms ranging from severe pelvic pain to infertility. It is characterized by growth of endometrial tissue outside of the uterine cavity. Diagnosis typically takes around 4-12 years due to the invasive nature of diagnostic surgery and widespread medical bias against female patients. Diagnosis is typically visually confirmed by presence of lesions after laparoscopic surgery, though imaging techniques such as ultrasound can also be used, while treatment is symptoms-based and typically involves progestin medication, NSAIDs, or hysterectomy. Endometriosis is grossly understudied, evident from the limited diagnostic and treatment options.

## Patheogenesis

The most widely accepted theories on patheogenesis of endometriosis are **dysfunction of the immune system and epigenetic factors**. Our model includes hormones and receptor binding dynamics to model these epigenetic factors and differences in hormone levels. Endometriosis lesions are able to locally synthesize $E_2$ from cholesterol, which may increase estrogen receptor (ER) activity and decrease progesterone receptor (PR) activity in endometrial and immune cells. This causes estrogen dependence and progesterone resistance, which has serious consequences for immmune cell function.

$ER_{\alpha}$ and $ER_\beta$ are nuclear receptors, meaning that they are found in the nucleus of the cell, where DNA transcription takes place. After $E_2$ binds to these receptors, different genes are transcribed, changing cell function. At normal levels of estrogen, the $ER_{\alpha}$ signaling pathway is dominant: $E_2$ binds to $ER_{\alpha}$ receptors, becoming bound $ER_{\alpha}$ complexes that pair into dimers. These $ER_{\alpha}$ dimers transcribe genes in the cell; in macrophages, for example, these genes control production of anti-inflammatory cytokines such as $IL-10$ and inhibition of inflammatory cytokines. At higher levels of $E_2$, the $ER_{\beta}$ signaling pathway is dominant: $E_2$ binds to both $ER_{\alpha}$ and $ER_{\beta}$ receptors on cells, where the bound $ER_{\alpha}$ and $ER_{\beta}$ combine into an $ER_\alpha -ER_\beta$ heterodimer, which is ineffective at gene transcription. In this way, $ER_{\beta}$ acts as an `off' switch for $ER_{\alpha}$. Consequently, high levels of $E_2$ result in production of pro-inflammatory cytokines in macrophages and other innate immune cells. However, individuals can also have different genetic affinities for which receptor is dominant: epigenetic factors have been found to increase $ER_\beta$ expression in endometrial cells.

$ER_{\alpha}$ upregulates PR function, meaning that the over-expression of $ER_{\beta}$ from local $E_2$ production in endometriotic lesions may cause the suppression of $ER_{\alpha}$ and of PRs downstream. In addition to inhibiting $ER_\alpha$ activity, $ER_\beta$ also interacts with cell machinery required for apoptosis to inhibit TNF- $\alpha$ induced cell death; consequently, despite stimulation of TNF- $\alpha$ by $ER_\beta$, lesion cells do not undergo typical apoptosis triggered by TNF- $\alpha$. Rather, TNF- $\alpha$ promotes inflammation through increased macrophage activity without causing lesion cell death. $ER_\beta$ also promotes lesion cell proliferation via CD47, a signaling protein typically expressed in healthy cells to protect them from being targeted by the immune system. This `don't eat me' signal is over-expressed in endometriotic cells due to the binding of $ER_\beta$ to the promoter region of CD47, protecting lesions from immune surveillance. **In both of these ways, $ER_\beta$ directly prevents clearance of lesion cells by the immune system and is heavily implicated in disease onset**: endometriotic tissue has been found to have ~ $100\times$ higher ratios of $ER_\beta$ to $ER_\alpha$ than healthy endometrial tissue, with amounts of $ER_\beta$ being directly linked to disease severity 

## Methods

We build upon pre-existing models: [Miller (2025)](https://doi.org/10.1098/rsif.2025.0076) and [Graham (2023)](https://doi.org/10.1016/j.mbs.2023.108979), adding our own modifications for estrogen receptor binding dynamics. We use ode15s in MATLAB R2024b to simulate a model containing (1) immune cell dynamics, (2) uterine cell profile, (3) steroid hormone levels, (4) pituitary hormone levels, and (5) estrogen receptors. We believe this model better reflects risk factors for disease onset and provides valuable insight into potential treatment efficacy.

## Results & Next Steps

So far, we've reproduced results from Miller and Graham (posted to [GitHub](https://github.com/suzannasem/endo)). We're currently working on our own modifications - stay tuned as these will be posted shortly!
