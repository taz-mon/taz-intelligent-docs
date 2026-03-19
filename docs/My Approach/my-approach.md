---
title: How I Work
excerpt: >-
  I'm an enthusiastic, detail-oriented principal tech writer with extensive
  experience writing documentation. 
deprecated: false
hidden: false
link:
  url: https://intelligent-documentation.readme.io/update/docs/my-approach
metadata:
  robots: index
---
I write about systems I use. Before documenting a Kubernetes (a container orchestration platform) configuration on different providers, I deploy an environment after configuring resources for it. Before explaining an API endpoint, I call it. This reveals gaps between what engineering intended and what a user actually encounters — and it's why the procedures I write tend to work the first time.

## Documentation as a system

I think the best documentation has a sensible structure, a conversational tone, and a rules-based process for keeping it accurate as the product changes.

At Pega, I designed the GitHub structure for Kubernetes deployment runbooks across six environments: AKS (Azure Kubernetes Service), EKS (Elastic Kubernetes Service), GKE (Google Kubernetes Engine), OpenShift, TKGI (Tanzu Kubernetes Grid Integrated Edition), and Minikube (a local Kubernetes cluster). Each runbook followed a consistent model so any developer, regardless of platform experience, could navigate directly to their environment without re-orienting. That structure is still in use.

At Legion Intelligence, as the sole writer, I build the help center from the ground up as features emerge or new sections become available in the UI. I work in a Docusaurus (a React-based static site generator) project managed in GitLab, with a branching workflow that supports multiple features in parallel. The process is repeatable, linear, manageable at speed, and structured like this:

1. Create a feature branch off main.
2. Clone it locally in VS Code.
3. Draft, review local builds with an LLM-based edit, commit updates, and push to the repository.
4. Complete the final review with reviewers using a merge request (MR).
5. Set the MR to auto-merge and squash after CodeRabbit (an AI-powered code review tool) completes its testing and approves the pipeline run.

## AI as a workflow layer

I use Claude (Anthropic's AI assistant) in two dedicated projects, each with a specific job.

### Drafting content project

I loaded my style guide into the project to create this environment, ensuring every initial draft starts from a consistent voice, structure, and terminology baseline. I capture configuration workflows on video using Loom (a screen recording tool), run the transcript through this project to generate a first draft, then refine it for technical accuracy. This cuts initial draft time significantly while keeping quality high.

### Git workflow project

This project has a Git-savvy instruction set I created for troubleshooting build issues and walking through the branch/clone/commit/push/MR sequence when merge conflicts arise. I use it to problem-solve hiccups — such as running `npm install` to align local builds with the latest package versions — so I don't have to pull in project engineers for build or Git questions. Having a repeatable checklist keeps me on top of my workflow when managing multiple feature branches simultaneously.

## Style governance that actually runs

At Pega, I contributed ideas to our Style Council. At Legion, I built the style guide from scratch, referencing industry-standard guides from Google, Kubernetes, and Red Hat. I published it in Confluence (Atlassian's team wiki) so anyone on the team can reference it when creating content. I then incorporate it into my drafting environment as an LLM (large language model) instruction prompt to enforce standards across all drafts and review edits. Wiring the style guide into the workflow is one of the best ways I know to automate documentation consistency.