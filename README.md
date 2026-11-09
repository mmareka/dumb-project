# Dumb Project (Lite)

A free, open-source project scheduler: task table, Gantt chart, critical path, resources and costs, with
files that move to Microsoft Project, Primavera P6, Jira and Inversion. It runs in the browser, needs no
install or account, and keeps your files on your own computer. Schedule Chicken, the helper in the
corner, adds and changes tasks from plain requests and answers questions about the schedule.

## Run it

- **Online:** https://mmareka.github.io/dumb-project/app/ (install it from Edge or Chrome to use it like a
  desktop app; `.sched` files then open with a double-click).
- **On your computer:** double-click `run_local.bat` (needs Python), or run
  `python -m http.server 5080` in this folder and open http://localhost:5080/app/.
- **Tests:** open http://localhost:5080/tests/.

## What it does

- Tasks, summary tasks, milestones; durations in hours, days, weeks or months
- Links of all four types with lag; constraints; critical path and float; circular-link warnings
- Calendar with work week, hours and holidays (one click adds US federal holidays)
- Resources with rates and max units, assignments, work and cost, over-booking warnings
- Progress, baselines, undo/redo, autosave, light and dark themes, Ctrl+K command list
- Drag bars to move them, drag the right edge to stretch, drag the dot onto another bar to link
- Schedule Chicken: "can we fit in three days of testing once build is done, Ana will handle it",
  "slide launch to next Monday", "what could make us miss the deadline?" It previews every change first,
  and every change can be undone.
- Open or drop in: `.sched`, Primavera P6 XER and P6 XML, Microsoft Project XML, Excel (.xlsx), CSV,
  Jira CSV export, and schedules inside documents: PDF reports, PowerPoint (tables or a drawn
  timeline), Word tables, pictures and scanned PDFs, shown for review before they become a schedule.
  Files are read in the browser and never uploaded; the PDF and text-recognition libraries ship with
  the app (see `app/vendor/README.md`). For a Microsoft Project .mpp, save it from Project as XML first.
- Save and export: `.sched`, Microsoft Project XML, Primavera P6 XER, CSV, Jira CSV, Inversion model and CSV

## License

MIT. See [LICENSE](LICENSE).
