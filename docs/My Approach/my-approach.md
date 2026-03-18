---
title: How I Work
excerpt: >-
  I'm an enthusiastic, detail-oriented principal tech writer with extensive
  experience writing documentation. 
deprecated: false
hidden: false
metadata:
  robots: index
---
I write about systems I use. Before documenting a Kubernetes configuration on different providers, I deployed an environment after configuring resources for it. Before explaining an API endpoint, I call it. This reveals gaps between what engineering intended and what a user actually encounters. It's why the procedures I write tend to work the first time.

## Documentation as a system

I think the best documentation has a sensible structure, a conversational tone, and a rules-based process for keeping it accurate as the product changes.

At Pega, I designed the GitHub structure for Kubernetes deployment runbooks across six environments: AKS, EKS, GKE, OpenShift, TKGI, and MiniKube. Each runbook followed a consistent model so any developer, regardless of their platform experience, could navigate directly to their environment without re-orienting. That structure is still in use.

At Legion Intelligence, as the sole writer there, I am building the help center from the ground up as features emerge or new sections become available in the UI. I work in a Docusaurus project managed in GitLab, with a branching workflow that supports multiple features in parallel. The process involves creating a feature branch off main, cloning it locally in VS Code, drafting and committing updates, and pushing, complete review via merge request, then engineering merges and squashes. Repeatable, linear, manageable at speed.

## AI as a workflow layer

I use Claude in two dedicated projects, each with a specific job.  

The first is a drafting environment loaded with my style guide, so every initial draft starts from a consistent voice, structure, and terminology baseline. I capture configuration workflows on video using Loom, run the transcript through this project to generate a first draft, then update it for technical accuracy. This cuts initial draft time significantly while keeping quality high.

The second is a process guide that walks me through the branch/clone/commit/push/MR sequence as a repeatable checklist when I'm managing multiple feature branches simultaneously.

## Style governance that actually runs

At Pega, I contributed ideas to our Style Council. At Legion, I built the style guide from scratch, referencing industry-standard guides from Google, Kubernetes, and Red Hat. I published it in Confluence so anyone on the team can reference it when creating content. I then incorporate it into my drafting environment as an LLM instruction prompt to enforce standards in all my drafts and review edits. Wiring it into the workflow is one of the best ways I know to automate documentation consistency.
