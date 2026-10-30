# macOS sidebar brand ink visual evidence

Captured in headless local Chrome on macOS against an isolated, real DSH Web host supplied by DSH Desktop 0.2.1-rc.5, with the PR build of dsh-claude-style 0.19.6.

After the normal web client started, the official Electron platform marker on the html element was set to darwin. Toggling the real sidebar caused its actual React component to render its macOS span branch. These are real host component screenshots, not a painted mockup or a screenshot of an Electron window.

Both states use brandInk=accent and customAccent=#e53935. Before captures restore only the two original button-restricted colour selectors in the loaded stylesheet. After captures use the PR stylesheet. No preference values or image pixels are changed between states.

Light/dark mode uses the host's data-ds-dark-theme marker. The repository privacy sanitizer runs before every screenshot; captures are cropped to the brand area and contain no workspace names, session contents, usernames, paths or tokens.

See evidence.json for the SPAN tag and computed colour readings. Screenshots are hosted on this separate evidence branch and are absent from the source PR and npm package.
