# PR 227: native sidebar status and context menu

These are actual cropped screenshots of the candidate build 1f032639c040 on a real isolated DSH Desktop 0.2.1-rc.5 Web host on macOS. Source base: 5259da9, product commit e58467f; a004663 changes only smoke expectations/probes and their generated inventory, not product output.

- running.png: the native ongoing indicator at the right edge.
- completed-menu.png: native background completion at the right edge, plus the original menu opened on that session without switching away from the selected conversation. The inline archive/pin buttons are absent; menu actions remain.

The current upstream custom paginated archive is retained. Its independent Unarchive action was exercised after archiving through the native menu. No manual-unread or subagent-session-tree code is included.

Fixture data comes from the real SessionController/SessionStore. A real native agent turn uses one scripted loopback model request, with no user model credentials. The repository privacy sanitizer ran before captures, and captures were reviewed. No private usernames, paths or tokens appear.

No verified equivalent before screenshot is supplied. A baseline source build was prepared, but the isolated host resolved the candidate client; the strict expected-build-id guard refused the capture and the incorrect before images were discarded. Existing source describes the baseline leading indicator and inline native controls. The after images above passed the exact candidate build-id check.

The evidence branch contains images and metadata only, outside the source PR and package.
