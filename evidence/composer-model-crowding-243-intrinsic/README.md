# PR 243 composer reflow evidence

Source before a759b1e (build 6b0bf6f5805d); after d1adf19 (build abc326397602).

All four images show the same real Flash selection, 700px middle column, 100% zoom and explicit 240 CSS px right-slot occupancy. The dashed pressure element is labelled non-account content. The captures are direct browser clips after privacy checks, with no resizing, redrawing or target-pixel edits. Clip coordinates and SHA256 values are in evidence.json.

- theme-before.png / theme-after.png: separate legitimate profile without the Codex model-slot takeover; other real plugins remain. This is the theme-owned model-picker case, not the original full user plugin combination.
- codex-before.png / codex-after.png: actual Codex priority -10 picker with the current real plugins. Before overlap/out-of-column targets disappear after this change.

Theme-owned results: baseline 5/14 geometry and 28/32 actions; candidate 14/14 and 32/32.
Codex-owned results: baseline 5/14 geometry and 29/33 actions; candidate 7/14 geometry and 33/33 actions. The remaining seven geometry failures are only the Codex private label-width rule (max-width min(360px,45cqw)); the PR does not alter that rule or falsely call the profile all-green.

Long transcript wheel scrolling, long draft caret, original width drag, header keyboard targets, scope/session transitions, native menus, actual model-directory changes and send/stop are exercised using only loopback model calls. All four test hosts shut down and the installed local package stayed unchanged.

This is actual shipped rc.5 frontend evidence in isolated DSH Web homes on macOS. It is not a physical Electron, Windows, phone or authenticated-quota test.
