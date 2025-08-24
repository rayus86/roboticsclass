# Robotics Class Repository (MVP)

This repository powers the curriculum site for Robotics 1 (and later Robotics 2).

## View the Site
GitHub Pages will publish automatically after merging the main branch (Actions workflow builds it).

## Local Development
1. Install Python 3.11+ (or 3.10+).
2. `pip install mkdocs-material`
3. Run: `mkdocs serve`
4. Open: http://127.0.0.1:8000

## Structure
```
docs/
  index.md
  robotics1/
  robotics2/
  reference/
  glossary.md
mkdocs.yml
```

## Adding Content
- Create a new markdown file under the correct folder.
- Add it to navigation in `mkdocs.yml`.
- Commit & push.

## Teacher Notes
Instructor-only comments are inside HTML comments `<!-- -->`. Keep solutions and answer keys in a private repo (not here).

## Next Steps (Planned)
- Add more R1 units (algorithmic thinking, CodeHS bridges)
- Add Arduino & Codrone pages
- Introduce design & CAD sections
- Expand Robotics 2 after R1 baseline stable