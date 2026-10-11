name: feature_request
description: Suggest a feature for AccessibleGoPro
body:
  - type: markdown
    attributes:
      value: |
        Thanks for suggesting an idea for AccessibleGoPro.

        Please describe the feature, why it's valuable for blind or low-vision users, and any accessibility concerns.
  - type: textarea
    id: summary
    attributes:
      label: Feature summary
      description: What is the feature you want?
      placeholder: Example: Add a spoken settings menu for resolution and frame rate.
    validations:
      required: true
  - type: textarea
    id: problem
    attributes:
      label: Problem or use case
      description: What problem does this solve for blind or low-vision users?
      placeholder: Example: A user wants to know the current recording mode and adjust it without looking at the camera screen.
    validations:
      required: true
  - type: textarea
    id: solution
    attributes:
      label: Proposed solution
      description: Describe how the app should behave.
      placeholder: Example: When the user navigates to settings, the app speaks the current option and speaks confirmation after selection.
    validations:
      required: true
  - type: textarea
    id: additional
    attributes:
      label: Additional context
      description: Add any relevant context, links, models, notes, or screenshots.
      placeholder: Optional
