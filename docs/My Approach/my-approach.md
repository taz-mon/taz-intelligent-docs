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

At Legion Intelligence, as the sole writer there, I am building the help center from the ground up as features emerge or new sections become available in the UI. I work in a Docusaurus project managed in GitLab, with a branching workflow that supports multiple features in parallel. The process is repeatable, linear, manageable at speed and structured like this:

1. Create a feature branch off main.
2. Clone it locally in VS Code.
3. Draft, review local builds with an LLM-based edit, commit updates, and push to the repository.
4. Complete the final review with reviewers using a merge request
5. I set the MR to be automatically merge and squash after code rabbit completes its internal testing and approves the pipeline run.

## AI as a workflow layer

I use Claude in two dedicated projects, each with a specific job.  

### Drafting content project

I loaded my style guide into the project to create this environment. This ensures that every initial draft starts from a consistent voice, structure, and terminology baseline. I capture configuration workflows on video using Loom, run the transcript through this project to generate a first draft, then update it for technical accuracy. This cuts initial draft time significantly while keeping quality high.

### Git workflow project

This project has a git-savvy instruction set that I created to be available for me to ask questions if my builds have trouble or for walking me through the branch/clone/commit/push/MR sequence if I ever get a merge conflict. This project helps me problem-solve hiccups, such as running npm install to align local builds with the latest package versions. This way, I don't have to bother project engineers with build or git questions and stay on top of my workflow. It's a reassurance to have a repeatable checklist when I'm managing multiple feature branches simultaneously.

## Style governance that actually runs

At Pega, I contributed ideas to our Style Council. At Legion, I built the style guide from scratch, referencing industry-standard guides from Google, Kubernetes, and Red Hat. I published it in Confluence so anyone on the team can reference it when creating content. I then incorporate it into my drafting environment as an LLM instruction prompt to enforce standards in all my drafts and review edits. Wiring it into the workflow is one of the best ways I know to automate documentation consistency.
