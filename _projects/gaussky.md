---
layout: page
title: gaussky
description: A lightweight simulator for Gaussian CMB and Galactic foreground sky maps at multiple frequencies.
importance: 2
category: "Cosmology & Inference"
---

{% include repository/project.html
   repository="liuyiqiandrew/gaussky"
   title=page.title
   description="Gaussian sky simulations specified by angular power spectra and spectral energy distribution models." %}

**Problem.** Testing a component-separation or inference method requires simulated skies with known statistical properties. A compact simulator makes it easier to study how an analysis responds to the assumed signal and foreground model.

**My work.** I built gaussky to generate multi-frequency Gaussian realizations of CMB and foreground maps. Sky components are specified through angular power spectra and spectral energy distribution models, connecting their spatial statistics to their frequency dependence.

**Scope and status.** The public repository contains the research implementation. Its Gaussian sky model provides a controlled setting for simulation studies; conclusions about more complex Galactic emission require additional tests with realistic foreground models.
