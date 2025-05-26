---
name: Custom issue template
about: Describe this issue template's purpose here.
title: Type
labels: ''
assignees: ''

---

name: 🐞 Bug Report
description: File a bug report
title: "[BUG]: "
labels: ["type: bug"]
assignees: []

body:
  - type: dropdown
    id: issue_type
    attributes:
      label: Type
      description: What type of issue is this?
      options:
        - Bug
        - Feature Request
        - Enhancement
        - Documentation
      default: 0
    validations:
      required: true

  - type: textarea
    id: what-happened
    attributes:
      label: What happened?
      description: A clear and concise description of the problem.
    validations:
      required: true
