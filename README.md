# Public Drift-Diffusion Models

This directory hosts two self-contained Jupyter notebooks illustrating drift–diffusion style models for sequential finger presses.

## Notebooks

### `single_press_model.ipynb`

Minimal model for a single  press decision with separate visual vs memory evidence streams. Produces basic reaction time (RT) and accuracy summaries across parameterized conditions.

### `sequence_model.ipynb`

Extends single-press model to sequences with different visual visiblities (visible horizon).
- models the effect of isolated violations in learned sequences

## Quick Start

1. Open a notebook in Jupyter / VS Code.
2. Run cells top-to-bottom. Figures and summary DataFrames will appear inline.

## Key Parameters (sequence model)

| Name | Meaning |
| ---- | ------- |
| `window` | Visible horizon (positions ahead) |
| `memory_drift_coef` | Base memory evidence strength |
| `visual_drift_coef` | Base visual evidence strength |
| `alpha`,`beta` | Decay / lateral inhibition coefficients |
| `threshold` | Planning completion bound |
| `visual_delay`,`motor_delay` | Stimulus vs execution latencies |

Adjust these to explore speed–accuracy tradeoffs.

## Citation
> **Integration of memory and sensory information in skilled sequence production**  
> Amin Nazerzadeh, Medha Porwal, J. Andrew Pruszynski, Jörn Diedrichsen  
> *bioRxiv* (2025). [https://doi.org/10.1101/2025.09.10.675426](https://doi.org/10.1101/2025.09.10.675426)


## License

MIT License

Copyright (c) 2025 Amin Nazerzadeh

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
