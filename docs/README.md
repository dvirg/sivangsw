GitHub Pages PDF Viewer

Steps to use

1. Copy the PDF file `מדריך לזכויות שמשפחות לא יודעות.pdf` into this `docs/` folder.
2. Commit and push the repo to GitHub.
3. In the repository settings on GitHub, enable GitHub Pages and set the source to `Deploy from: Branch: main` and `Folder: /docs` (or select `docs` if available).
4. After Pages is built, open the site URL and you'll see `index.html` which uses PDF.js to render the PDF.

Testing locally

- Using Python 3:

```powershell
cd docs
python -m http.server 8000
# then open http://localhost:8000 in your browser
```

- Or using Node (if you have http-server):

```powershell
cd docs
npx http-server -p 8000
# then open http://localhost:8000
```

Notes

- Do NOT commit sensitive files to the repo. The PDF may contain private content; if so, host it on a private Pages branch or a private file host.
- If the PDF filename changes, update `index.html` to match the filename or rename the file to the expected name.
