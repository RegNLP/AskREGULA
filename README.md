# AskREGULA

A browser-based UI toolkit for the AskREGULA regulatory QA benchmark platform. It provides three distinct consoles — an End User workspace, an Admin Console, and an Expert Review Console — all accessible from a single landing page.

---

## Project Structure

```
AskREGULA/
├── index.html                           # Landing page — links to all three consoles
├── images/                              # Logos and icons
├── styles/
│   ├── admin-console.css                # Styles for the Admin Console
│   ├── askregula-end-user-workspace.css # Styles for the End User Console
│   └── expert-review.css               # Styles for the Expert Review Console
└── ui/
    ├── admin/
    │   └── adminUI.html                # Admin Console — open directly in browser
    ├── enduser/
    │   └── enduserUI.html              # End User workspace
    └── review/
        └── expertUI.html               # Expert Review Console
```

---

## Consoles

| Console | File | Description |
|---|---|---|
| End User | `ui/enduser/enduserUI.html` | Query interface for asking regulatory questions |
| Admin | `ui/admin/adminUI.html` | Manage corpora, benchmarks, runs, and versions |
| Expert Review | `ui/review/expertUI.html` | Annotation interface for expert reviewers |

---

## Running the Project

All files are self-contained and can be opened directly in a browser. The simplest way is to serve the project with a local http server so relative paths resolve correctly:

```sh
cd /path/to/AskREGULA
python3 -m http.server 8000
```

Then open [http://127.0.0.1:8000/index.html](http://127.0.0.1:8000/index.html)

Alternatively, open the individual HTML files directly from the `ui/` folders.