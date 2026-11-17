# ReleasePilot AI: public demo website

Static build of ReleasePilot AI (Karan Deshmukh, MSc ESAIP) for the public demo link.
This branch holds only the website and is deployed to Vercel. It is unrelated to the BizAssist code on `main`.

| File | What it holds |
|---|---|
| `index.html` | The app: its styles, its data, and its code |
| `lib/` | The libraries that write Word, PDF, and Excel files. The page loads them as separate files, so a browser keeps them between visits. |
| `docs/` | The published documents. The app fetches one only when a visitor opens it: the PDF files as they are, and the Word and Excel files from `office.json`. |

The documents were once embedded in `index.html`, which made the page 8 MB and slow to open on a phone. The page is now 1.7 MB, and the documents load on demand.
