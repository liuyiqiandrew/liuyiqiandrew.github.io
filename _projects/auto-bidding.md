---
layout: page
title: Sequential Auto-Bidding
description: PPO agents for replay-based auctions with budget constraints and changing market conditions.
importance: 2
category: "AI & Machine Learning"
---

{% include repository/project.html
   repository="liuyiqiandrew/AuctionNet"
   title=page.title
   description="Reinforcement-learning experiments built on the AuctionNet auto-bidding benchmark." %}

**Problem.** An automated bidder makes a sequence of decisions under budget and cost-per-action constraints. Good decisions depend on both the current auction and how spending affects opportunities later in the episode.

**My contribution.** I developed PPO agents in a replay-based auction environment, extending their observations and policies with temporal stacking and recurrent representations. I used controlled experiments and ablations to study reward shaping, market-state features, and policy architectures under changing market conditions.

**Context and status.** This work was part of a group project for COS 435, Introduction to Reinforcement Learning, at Princeton in Spring 2026. The repository builds on the AuctionNet benchmark and includes the group's broader PPO and LLM experiments; the work described here focuses on my PPO contributions.
