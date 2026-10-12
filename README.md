# Dong Yoon Lee — Academic Website

Static GitHub Pages site for <https://dlee267.github.io>.

## Content structure

- `index.html` — research overview, selected work, education, and recognition
- `publications.html` — peer-reviewed papers, preprint, and patent
- `cv.html` — master CV overview and embedded PDF
- `contact.html` — public contact and scholarly profiles
- `work/multimodal-ai.html` — multimodal AI and foundation models
- `work/health-sensing.html` — connected health and activity sensing
- `work/physical-computing.html` — adaptive structures and embedded sensing
- `work/environmental-sensing.html` — air quality and environmental prediction
- `assets/dong-yoon-lee-cv.pdf` — public master CV

## Source of truth

The content was derived from:

```text
/home/dongyoon/projects/resume/cv/dong_yoon_lee_cv.typ
```

When the master CV changes, rebuild it in the resume repository and replace the public PDF:

```bash
typst compile --root . cv/dong_yoon_lee_cv.typ cv/dong_yoon_lee_cv.pdf
cp cv/dong_yoon_lee_cv.pdf /home/dongyoon/projects/dlee267.github.io/assets/dong-yoon-lee-cv.pdf
```

Update the relevant HTML pages whenever publication metadata, project results, contact details, or awards change.

## Local preview

```bash
python3 -m http.server 8765 --bind 127.0.0.1
```

Then open <http://127.0.0.1:8765/>.

## Deployment

The repository is a dependency-free static site. Commit and push changes to the GitHub Pages publishing branch configured for the repository.
