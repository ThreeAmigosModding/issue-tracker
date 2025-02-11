---
name: Bug Report
about: Report a bug in one of our projects
labels: [bug]
body:
  - type: markdown
    attributes:
      value: "## 🐛 Bug Report"
  - type: textarea
    id: description
    attributes:
      label: "Describe the Bug"
      description: "A clear and concise description of what the bug is."
    validations:
      required: true
  - type: textarea
    id: reproduction_steps
    attributes:
      label: "Steps to Reproduce"
      description: "Steps to reproduce the behavior."
      placeholder: "1. Go to '...'
2. Click on '...'
3. Scroll down to '...'
4. See error"
    validations:
      required: true
  - type: textarea
    id: expected_behavior
    attributes:
      label: "Expected Behavior"
      description: "A clear and concise description of what you expected to happen."
    validations:
      required: true
  - type: textarea
    id: logs
    attributes:
      label: "Logs & Console Output"
      description: "Paste any relevant logs or error messages."
      render: shell
  - type: textarea
    id: screenshots
    attributes:
      label: "Screenshots"
      description: "If applicable, add screenshots to help explain your problem."
      placeholder: "![](https://example.com/screenshot.png)"
  - type: dropdown
    id: resources
    attributes:
      label: "Impacted Resource"
      description: "Which resources are impacted by this issue?"
      multiple: true
      options:
        - Advanced Fuel
        - Advanced Police Job
        - Elevator
        - Tire Slash
        - Scoreboard
        - Bug Report
        - Fire Danger Signs
        - Changelog
        - Radio Animations
        - ChatToolBox
        - Simple Blip Management
  - type: input
    id: artifact_version
    attributes:
      label: "Artifact Version"
      description: "Specify the version of the artifact where the issue was found."
      placeholder: "e.g., 12307"
    validations:
      required: true
  - type: input
    id: game_build
    attributes:
      label: "Game Build Number"
      description: "Provide the game build number where the issue occurs."
      placeholder: "e.g., Build 3258"
    validations:
      required: true
  - type: textarea
    id: additional_info
    attributes:
      label: "Additional Information"
      description: "Add any other context about the problem here."
---
