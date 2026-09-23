---
layout: page
title: Foreground Template Fitting
description: Weighted fits to polarized sky maps, with harmonic filtering and Monte Carlo uncertainty propagation.
importance: 1
category: "Cosmology & Inference"
---

{% include repository/project.html
   repository="liuyiqiandrew/fg_weighted_template_fit"
   title=page.title
   description="Python estimators for weighted foreground template fits to HEALPix Q/U maps." %}

**Problem.** Polarization maps contain a mixture of cosmological signal, Galactic emission, and instrument noise. Comparing maps at different frequencies requires accounting for their resolution and for noise in both the observations and the foreground templates.

**My work.** I developed a Python package that matches maps to a common beam, optionally filters angular modes, constructs foreground templates from map differences, and estimates their amplitudes with weighted fits. Independent template realizations support cross-template estimators, while Monte Carlo noise realizations propagate uncertainty through template construction and fitting.

**Scope and status.** This is research software with tests and usage documentation in the repository. The estimator uses diagonal pixel weights. Its results depend on the chosen sky region, filtering, templates, and noise model, so these choices are part of the analysis and its validation.
