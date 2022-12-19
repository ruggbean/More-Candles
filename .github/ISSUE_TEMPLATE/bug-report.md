name: Bug Report
description: File a bug report
title: "[Bug]: "
labels: ["bug"]
assignees:
  - ruggbean
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!
  - type: dropdown
    id: version
    attributes:
       label: Mod Version
      description: What version of More Candles are you reporting?
      options:
        - 1.0.0
        - 1.0.1
        - 1.0.2
        - 1.0.3
    validations:
      required: true
  - type: textarea
    id: mods
    attributes:
      label: Modded
      description: Do you have other mods installed? If so, which mods and versions?
      placeholder: i.e., Expanded Foods 1.6.4, A Culinary Artillery 1.0.10, etc.
    validations:
      required: true
  - type: dropdown
    id: type
    attributes:
      label: SP/MP
      description: Did you experience this issue in singleplayer or multiplayer?
      options:
        - Singleplayer
        - Multiplayer
    validations:
      required: true
  - type: textarea
    id: what-happened
    attributes:
      label: Description
      description: Explain the issue you're running into.
      placeholder: Please be as detailed as necessary for me to understand the problem.
      render: shell
    validations:
      required: true
  - type: textarea
    id: repro
    attributes:
      label: How to Reproduce
      description: Explain how we could reproduce your bug/issue.
      placeholder: Please be as detailed as necessary for me to understand the problem.
      render: shell
    validations:
      required: false
  - type: textarea
    id: screens
    attributes:
      label: Screenshots
      description: Attach a screenshot if it helps explain the issue / shows a visual bug.
      placeholder: Drag and drop pictures here
      render: shell
    validations:
      required: false
  - type: textarea
    id: logs
    attributes:
      label: Logs
      description: In the game's Logs folder you may be able to find more information inside client-main.txt and server-main.txt. Alternatively, you may use gist.github.com to upload logs, linking them here, if they're too large.
      placeholder: Paste crash between the triple backticks
      value: ```Log```
      render: shell
    validations:
      required: false

