# Coasty CUA v1 — OSWorld Showcase

Real desktop tasks completed end-to-end by **Coasty CUA v1** on the
[OSWorld](https://os-world.github.io/) benchmark — image editing, office
suites, the browser, the operating system, email, media, and
cross-application workflows.

Every task page includes the original instruction, a screenshot of the
final state, the full screen recording, the per-step trajectory (actions,
reasoning, screenshots), and the original OSWorld task definition.

## Domains

- [**Chrome**](./chrome/README.md) — Browser navigation, tab management, and web-based workflows.
- [**GIMP**](./gimp/README.md) — Image editing, color manipulation, layer operations, and export.
- [**LibreOffice Impress**](./libreoffice_impress/README.md) — Slide creation, formatting, transitions, and presentation export.
- [**LibreOffice Writer**](./libreoffice_writer/README.md) — Document authoring, formatting, styles, and structural edits.
- [**Multi-app Workflows**](./multi_apps/README.md) — Cross-application workflows that span the browser, editors, terminals, and the file manager.
- [**Operating System**](./os/README.md) — System-level operations: file management, terminal commands, settings, and configuration.
- [**Thunderbird**](./thunderbird/README.md) — Email composition, account configuration, filtering, and folder management.
- [**VLC**](./vlc/README.md) — Media playback, conversion, subtitle handling, and playlist operations.
- [**VS Code**](./vs_code/README.md) — Extension management, settings, code edits, terminal use, and Git operations.

## Run setup

- **Action space:** `pyautogui` (Python automation primitives)
- **Observation:** screenshot
- **Provider:** AWS
- **Resolution:** 1920×1080

## Layout

```
results/
├── README.md                  ← this file
├── <domain>/
│   ├── README.md              ← list of completed tasks for the domain
│   └── <task_id>/
│       ├── README.md          ← instruction + final screenshot + links
│       ├── recording.mp4      ← full screen recording of the run
│       ├── traj.jsonl         ← per-step action / reasoning / screenshot
│       ├── runtime.log        ← runtime log
│       ├── result.txt         ← evaluator score
│       ├── task.json          ← original OSWorld task definition
│       └── step_*.png         ← all per-step screenshots
```
