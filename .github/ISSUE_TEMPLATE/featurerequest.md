---
name: FeatureRequest
about: For submitting feature requests
title: "[Feature]:"
labels: ''
assignees: ''

---

name: FeatureRequest
description: File a feature request
title: "[Feature]: "
labels: ["enhancement", "triage"]
assignees:
  - qinhao77-create
body:
  - type: markdown
    attributes:
      value: |
        Thanks for suggesting a new feature!
  - type: input
    id: requester-name
    attributes:
      label: Your Name
      description: Who is requesting this feature?
      placeholder: ex. Qin Hao
      required: true
  - type: dropdown
    id: os
    attributes:
      label: Target Operating System
      description: Which OS is this feature for?
      options:
        - Windows
        - macOS
        - Linux
        - Cross-platform
  - type: textarea
    id: feature-description
    attributes:
      label: Feature Description
      description: What feature would you like to see added?
      placeholder: Describe the feature in detail
      required: true
  - type: textarea
    id: use-case
    attributes:
      label: Use Case
      description: How would this feature help you or other users?
      placeholder: Explain the use case or scenario
  - type: checkboxes
    id: terms
    attributes:
      label: Agreement
      description: By submitting this request, you confirm you've read the contribution guidelines.
      options:
        - label: I agree to follow the project's contribution guidelines
          required: true
