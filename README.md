# Gradient Descent Demo

This project is a compact, visual demonstration of optimization with gradient descent on a 2D quadratic cost function.

## Objective

The notebook minimizes:

\[
J(w_1, w_2) = w_1^2 + 2w_2^2
\]

Its gradient is:

\[
\nabla J(w) = [2w_1,\ 4w_2]
\]

Because the curvature is different in each direction, this function is a good example for showing how optimizer settings affect convergence behavior.

## Notebook Content

The notebook `gradient_descent_demo.ipynb` includes:

1. **Base setup**: imports and definitions of the cost function and gradient.
2. **Vanilla gradient descent implementation**.
3. **Contour path visualization** for a single learning rate.
4. **Learning-rate comparison** (`0.001`, `0.01`, `0.1`) plotted on the same contour map.
5. **Convergence diagnostics**: cost vs iteration curves on a log scale.
6. **Momentum vs Vanilla GD** comparison:
   - trajectory on contour lines,
   - cost-vs-iteration plot,
   - final numeric cost printout.

## Why This Adds Value

- Moves beyond lecture copy by comparing optimizer behavior, not just running one case.
- Shows both **geometric intuition** (contour paths) and **quantitative evidence** (cost curves).
- Demonstrates a practical optimizer extension (momentum) used in real ML training.

## How to Run

1. Open `gradient_descent_demo.ipynb` in VS Code or Jupyter.
2. Select the project virtual environment kernel (`.venv`).
3. Run cells from top to bottom.

Required packages:
- `numpy`
- `matplotlib`

## Suggested Next Improvements

- Add an automatic stopping criterion based on gradient norm (instead of fixed steps).
- Add a small results table (`method`, `learning_rate`, `steps`, `final_cost`).
- Add a short markdown interpretation after each plot (2–3 lines) to explain the behavior.

## Project Structure

- `gradient_descent_demo.ipynb` — main demo notebook
- `README.md` — project documentation
