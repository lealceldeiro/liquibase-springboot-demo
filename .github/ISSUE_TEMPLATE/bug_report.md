name: Bug Report
description: File a bug report
title: "[Bug] "
labels: ["bug"]
assignees:
  - lealceldeiro
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!
  - type: input
    id: contact
    attributes:
      label: Contact Details
      description: How can we get in touch with you if we need more info?
      placeholder: (optional) ex. email@example.com
    validations:
      required: false
  - type: textarea
    id: what-happened
    attributes:
      label: What happened?
      description: Also tell us, what did you expect to happen?
      placeholder: Tell us what you see!
      placeholder: "A bug happened!"
    validations:
      required: true
  - type: dropdown
    id: device-type
    attributes:
      label: Device
      description: What device are you using to visit our blog?
      options:
        - Desktop (PC, Laptop, etc.)
        - Mobile (Android)
        - Mobile (iOS)
    validations:
      required: true
  - type: dropdown
    id: browser-type
    attributes:
      label: Browser
      description: What browser are you using to visit our blog? (You could [search how to know that](https://duckduckgo.com/?q=how+to+know+what+browser+i'm+using) or visit [https://www.whatsmybrowser.org/](https://www.whatsmybrowser.org/))
      options:
        - Google Chrome (Default)
        - Mozilla Firefox
        - Microsoft Edge
        - Vivaldi
        - Safari
        - Opera
        - Maxthon
        - Avast Secure
        - Avant
    validations:
      required: true
  - type: input
    id: browser-version
    attributes:
      label: Browser version
      description: Version of the browser you're using to visit out blog (Again, you could [search how to know that](https://duckduckgo.com/?q=how+to+know+my+browser+version) or visit [https://www.whatsmybrowser.org/](https://www.whatsmybrowser.org/))
      placeholder: ex. 94.0 (64-bit)
    validations:
      required: false
  - type: textarea
    id: logs
    attributes:
      label: Relevant log output
      description: Please copy and paste any relevant log output. This will be automatically formatted into code, so no need for backticks.
      render: shell
  - type: checkboxes
    id: terms
    attributes:
      label: Code of Conduct
      description: By submitting this issue, you agree to follow our [Code of Conduct](https://github.com/lealceldeiro/org.wcdevs.blog.front/blob/main/CODE_OF_CONDUCT.md)
      options:
        - label: I agree to follow this project's Code of Conduct
          required: true
