**Blended FDM: Digital Material Filament Visualization**

This repository contains the Python code for a university project in "Non-Traditional Manufacturing Processes." The project explores the concept of Blended Fused Deposition Modeling (b-FDM) by modeling and visualizing a "Digital Material" (DM) filament capable of producing functionally graded materials from a single-nozzle 3D printer.

**Project Context & Inspiration**

The core methodology is inspired by the 2024 Nature Communications article:

"3D printing with a 3D printed digital material filament for programming functional gradients"
by Sang-Joon Ahn, Howon Lee & Kyu-Jin Cho.
https://doi.org/10.1038/s41467-024-47480-5

**Core Concept**

The b-FDM process involves 3D printing a custom filament (a DM filament) composed of two or more base materials (e.g., Material A and Material B). This DM filament has a specific, pre-programmed cross-sectional composition along its length.

When this DM filament is fed back into a standard FDM printer, the base materials blend in the nozzle. This results in a final printed object with a programmed functional gradient (e.g., color, stiffness) without requiring a complex multi-nozzle printer.

**What This Code Doe**s

This project models and visualizes the composition of both the DM filament and the final 3D object for a 40mm cube with a vertical material gradient (from 100% Material A at the bottom to 100% Material B at the top).

The main Jupyter Notebook (me323_project-Copy1.ipynb) and standalone scripts provide:

**DM Filament Composition Modeling:**

Calculates the required cross-sectional composition (Material A vs. B) of the DM filament for each layer of the final cube.

Implements models for both Linear and Quadratic (ease-in) material gradients.

**DM Filament Visualization:**

Cross-Section: Generates a plot of the DM filament's cross-section, showing the distribution of Material A (Blue) and Material B (Red) at any given layer of the final print.

Side View: Generates a stacked bar chart visualizing the total length of Material A and B required within each of the DM filament's internal layers to produce the entire graded object.

**Final Object Visualization:**

Matplotlib Sliced View: Renders a 3D view of the final cube built from thin, stacked layers, each colored according to the programmed gradient.
