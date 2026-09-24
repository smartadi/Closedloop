# Manuscript figures — source of truth

The **canonical, finalized main paper figures live in the brain_paper repo**, in

```
brain_paper/paper/figures_final/FigureN.pdf      (N = 1..5)
```

assembled in Illustrator from the locked panel set under
`figures_final/panels/<figure>/` (see `figures_final/MANIFEST.txt` +
`collect_final_panels.m`). Those are the actual paper figures.

The `images/FigureN.pdf` here are **copies** of that canonical set, kept in this
repo only because Overleaf compiles from local files. To refresh after a figure is
re-assembled, copy it over with the same clean name, e.g.

```
cp ../brain_paper/paper/figures_final/Figure3.pdf images/Figure3.pdf
```

Conventions:
- Use the clean name `images/FigureN.pdf` in `\includegraphics` — **no `_extra` suffix**
  (the old `Figure2_extra.pdf` / `Figure3_extra.pdf` were retired 2026-09-23).
- Figures 1, 2, 3, 5 are single assembled PDFs from `figures_final`.
- Figure 4 is still built in `results.tex` from separate panel files
  (`f4_reject_pooled.pdf`, `f4_error_decomp.png`, `f4_error_exemplars.png`) pending
  its Illustrator assembly; swap to `images/Figure4.pdf` from `figures_final` once final.
