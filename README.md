# Local sidebar prototype evidence

These are actual cropped browser screenshots from an isolated DSH Desktop 0.2.1-rc.5 Web host on macOS, using a locally modified dsh-claude-style 0.19.6 build. They are not screenshots of the current upstream 0.19.7 source, and are not Electron-window captures.

The viewport was 1280 x 860. Captures were sanitized before writing and reviewed; only demo session titles and workspace names appear.

- native-running-right.png and native-completed-right.png: real native agent runtime, with the model served by a loopback scripted endpoint. No production model credits were used. Native state nodes and priority remain unchanged; the existing indicator is positioned on the right.
- context-menu.png: real native SessionController/SessionStore records and native menu actions. Right-clicking a background session opens the same menu as the ellipsis without selecting the session. Only the native inline archive/pin slot cells are suppressed; the corresponding menu commands remain.

The context screenshot also shows an independent local manual-unread item. Manual unread is outside the proposed three-feature scope. No subagent-session grouping is included.

Validation of the local prototype: 13 right-status mechanism tests, 12 context-menu mechanism tests, and 462 tests in the full local suite; all local verify gates passed. The full suite also includes other local work. These results do not claim validation against the latest upstream source or physical Windows execution. The context build id is e32f9cb4af80.

This branch contains visual evidence only, not an implementation pull request. CONTRIBUTING.md asks feature/layout changes to start with an issue and wait for a maintainer response.
