---
layout: page
title: Terminal-Bench-Science
description: Scientific tasks that evaluate how AI agents build, test, and revise models in computational research.
importance: 1
category: "AI & Machine Learning"
---

{% include repository/project.html
   repository="harbor-framework/terminal-bench-science"
   title=page.title
   description="A collaborative benchmark for AI agents working on real-world scientific workflows." %}

**Problem.** A model can fit the data available to an agent while relying on assumptions that fail in other settings. Evaluating scientific reasoning requires testing whether the agent's model generalizes and whether its analysis is reproducible.

**My contribution.** I contribute scientific tasks and reviews to Terminal-Bench-Science. I authored a CMB inference benchmark centered on model misspecification: restrictive assumptions can remain statistically adequate on observed data while failing under held-out evaluation conditions. I also review astronomy and physics tasks for scientific validity, difficulty, verifier robustness, reproducibility, and potential shortcuts.

**Status.** This is an ongoing contribution to a collaborative project, beginning in 2026. The linked upstream repository contains the benchmark, contribution guidelines, and current development activity.
