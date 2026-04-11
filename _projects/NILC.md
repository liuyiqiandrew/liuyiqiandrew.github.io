---
layout: page
title: Needlet ILC
description: A method for combining multi-band sky maps to isolate a faint target signal from contamination and instrument noise.
img: assets/img/12.jpg
importance: 1
category: ordered
---
<div class="repo-ticket-card">
  <a class="repo-ticket-card__anchor" href="https://github.com/liuyiqiandrew/NILC" target="_blank" rel="noopener noreferrer">
    <span class="repo-ticket-card__title">Needlet ILC</span>
    <span class="repo-ticket-card__row">
      <span class="repo-ticket-card__name">liuyiqiandrew/NILC</span>
      <span class="repo-ticket-card__platform">GitHub</span>
    </span>
    <span class="repo-ticket-card__divider" aria-hidden="true"></span>
    <span class="repo-ticket-card__description">Needlet ILC implementation, source code, and supporting experiments.</span>
  </a>
</div>

<p><strong>Problem.</strong> When a telescope observes the sky in several frequency bands, each map contains a mixture of things you want and things you do not want. In this case, the target is the cosmic microwave background, while the unwanted parts include Galactic emission, point sources, and detector noise. The challenge is to combine the maps so that the shared target signal remains while the contamination is reduced as much as possible.</p>

<p><strong>Method.</strong> ILC stands for <em>internal linear combination</em>. The basic idea is simple: take a weighted average of several input maps, choose the weights so the target signal is kept unchanged, and at the same time make the overall unwanted variation as small as possible. Needlet ILC adds another layer by splitting the maps into wavelet-like pieces called <em>needlets</em>, so the weights can change with both spatial scale and sky location. In practice, that makes the method more adaptive when contamination behaves differently in different parts of the data.</p>

<p><strong>Strengths.</strong> NILC is flexible, fairly intuitive, and does not require a very detailed physical model of every contaminating signal. It can work especially well when the unwanted emission changes from place to place or from large-scale structure to small-scale structure, because the weights are allowed to adapt instead of being fixed everywhere.</p>

<p><strong>Limitations.</strong> The method depends on estimating correlations in the data well, so it can struggle when the inputs are very noisy, when there are too few frequency channels, or when the channels are not well matched. In those cases it may leave residual contamination behind or place too much weight on noisy data. In this implementation, the method behaves reasonably on cleaner intensity-like maps, but it is less robust on older, noisier WMAP-like data and remains a work in progress.</p>
