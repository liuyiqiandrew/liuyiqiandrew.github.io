---
layout: page
title: Needlet ILC
description: Needlet-domain component separation for combining sky maps across frequencies and spatial scales.
importance: 3
category: "Cosmology & Inference"
---
{% include repository/project.html
   repository="liuyiqiandrew/NILC"
   title=page.title
   description="Needlet ILC implementation, source code, and supporting experiments." %}

**Problem.** Each frequency map of the sky contains a mixture of CMB signal, Galactic emission, point sources, and detector noise. Component separation combines these observations to preserve the CMB while reducing contamination.

**My work.** During my undergraduate research with CLASS, I implemented and optimized a needlet-domain minimum-variance estimator. Internal linear combination (ILC) chooses frequency weights that preserve the target signal while minimizing the variance of the combined map. Needlets allow those weights to vary with spatial scale and sky location, adapting to changing foreground conditions.

**Scope and status.** This repository contains the research implementation and supporting experiments. Its performance depends on estimating correlations reliably and matching the input maps. The existing implementation is less robust on noisy WMAP-like data and should be treated as research code with those limitations.
