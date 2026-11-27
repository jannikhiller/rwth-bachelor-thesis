# Model Checking Stochastic Games with Storm

My bachelor's thesis at RWTH Aachen studies almost-sure reachability in stochastic
multiplayer games: can a coalition reach a target with probability one, regardless
of the other players' strategies?

I formalized a nested fixed-point algorithm, proved its correctness and
Θ(nm) time complexity, and implemented a layered inner-loop optimization in Storm.
The thesis reports speedups of 5–25× over PRISM-games in its experimental evaluation,
particularly for smaller inputs; these measurements apply to the evaluated benchmarks.

**[Read the reconstructed thesis PDF](preview/rebuilt-preview.pdf)** ·
[Storm implementation](https://github.com/jannikhiller/storm) ·
[Experiment scripts and benchmarks](https://github.com/jannikhiller/rwth-bachelor-thesis-storm-tests)

## Source and PDF provenance

Bachelor's thesis source recovered from Overleaf exports.

- `main.tex`: most complete thesis source, including the evaluation and conclusion. Build with pdfLaTeX, BibTeX, and additional pdfLaTeX passes.
- `presentation/`: thesis presentation; `earlier-export/` retains a differing earlier export.
- `drafts/`: earlier thesis-source revisions.
- `preview/rebuilt-preview.pdf`: reconstructed preview, not the original submitted PDF. The source inserts the build date on its cover.

The implementation is in [the Storm fork](https://github.com/jannikhiller/storm); experiment scripts are in [rwth-bachelor-thesis-storm-tests](https://github.com/jannikhiller/rwth-bachelor-thesis-storm-tests).
