# The attractor — Module XII

Standalone interactive extract of Module XII, "The attractor", from the Chronowave Dynamics Temporal Engine: a single-file compendium of 17 interactive modules about the author's temporal framework. The full compendium, its manual and its edit log are in [chronowave-compendium](https://github.com/Ajuntanaga/chronowave-compendium). The module's own heading on the page reads: "Where it all began: pulses on a Lorenz attractor".

## Use it

Download or clone this repository, then open [`Module_XII_Attractor.html`](Module_XII_Attractor.html) from disk in a current browser (GitHub only shows its source). There is no build step and nothing to install. Math (KaTeX 0.16.9) and fonts load from cdnjs and Google Fonts, so equations and typography need a connection.

## Files

| File | What it is |
|---|---|
| [`Module_XII_Attractor.html`](Module_XII_Attractor.html) | The module: one page with the shared styles, this module's section and the script statements it needs. |
| [`Module_XII_Manual.md`](Module_XII_Manual.md) | This module's part of the compendium's plain-text manual (extracted from rev b90 and hand-patched, so it may lag the page). |

The other two files are this README and a `.gitignore`.

## Where it comes from

Made on 2026-11-14 from rev b91 of the compendium page (commit `6cf22d4` of chronowave-compendium) by the scripts in the `tools/split` folder of that repository (added in later commits). The section markup, the styles and the script statements are copied from the page without change. What differs is the page title and description, a short header and footer line and small stand-ins for the parts of other modules that this module reads (see the limits below).

## Checks and limits

- A scripted headless-Chromium test loaded the page, moved every slider, select and checkbox, clicked every button and sent pointer, wheel and key events to every canvas: 79 actions (slider moves, clicks, and pointer, wheel and key events), 1 canvas, no uncaught exception and no console error. It is a smoke test: this extract was not compared with the original module for identical behaviour, and nothing here has had an independent review.
- The sigma, rho and beta sliders, the Lyapunov and twin-separation readouts, the time fold, the Drive control and the 3-D canvas are this module's own and work here.
- The number of wings comes from the scale selected on the lattice of Module IV; here the scale is fixed at its start-up one (seven selected notes), so there are always seven wings.
- The drive is always built from a stack interval of 4 semitones (the value Module XIII starts with); the readout next to the Drive slider also shows 261.6 Hz, which comes from A4 = 440 Hz and does not enter the drive.
- "TFE couple" can be switched on, but the field-equation solver it reads from (Module X) is not here, so it adds nothing to rho (read from the code; the button was only clicked in the test).
- The framework is the author's own and still in progress; Module XVII of the compendium (also a repository of its own, [chronowave-verdicts-and-rulings](https://github.com/Ajuntanaga/chronowave-verdicts-and-rulings)) carries the page's own verdicts and open rulings.
- No license: all rights are reserved by default, beyond viewing and forking on GitHub; a license is the author's decision.
