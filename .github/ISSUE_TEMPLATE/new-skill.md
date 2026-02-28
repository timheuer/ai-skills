name: "🧰 New Skill Proposal"
description: "Use this form to propose a new Skill with clear intent and scope."
title: "[Skill]: "
body:

- type: markdown
    value: |
      Thanks for proposing a new Skill/Tool/Agent! Please fill out the fields below thoughtfully.
      This helps maintainers understand the idea, scope, and impact before implementation.

- type: input
    id: summary
    attributes:
      label: "1. One-Sentence Summary"
      description: "Describe the capability in one sentence."
      placeholder: "E.g., Adds authentication scaffolding to ASP.NET projects."
      required: true

- type: textarea
    id: problem_statement
    attributes:
      label: "2. Problem Statement"
      description: |
        What problem does this solve?
        • Who is the user?
        • What are they trying to accomplish?
        • What pain does this remove?
      placeholder: "Describe the user problem."
      required: true

- type: textarea
    id: trigger_context
    attributes:
      label: "3. Trigger Context"
      description: |
        When should this Skill/Tool activate?
        Provide example prompts or signals that should trigger it.
      placeholder: "E.g., ‘Add auth’, ASP.NET project detected…"
      required: true

- type: input
    id: proposed_name
    attributes:
      label: "4. Proposed Name"
      description: "Suggested canonical name — should be discoverable and scoped."
      placeholder: "e.g., auth-scaffold-aspnet"
      required: true

- type: textarea
    id: alternatives
    attributes:
      label: "5. Alternatives Considered"
      description: "Why not handled by existing Skill/Tool/Docs?"
      placeholder: ""
