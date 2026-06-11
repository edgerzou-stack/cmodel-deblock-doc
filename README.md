# C-Model Deblock Documentation Dashboard

This repository contains an interactive HTML dashboard documenting the C-Model Deblocking (去块滤波) architecture, primarily focusing on HEVC/VVC standards as implemented in the KHEnc codebase.

## Features

- **Interactive Navigation**: Sidebar and Top Navigation to easily browse through the architecture.
- **Mermaid Flowcharts**: Visualizes the CTU-level pipeline and Boundary Strength (BS) decision logic.
- **Physical Pixel Layouts**: Custom CSS diagrams mapping the physical pixel positions (e.g., `p0`, `q0`) to their C-Model array pointer representations (e.g., `p[0]`, `p[-1]`).
- **Core Filtering Formulas**: Detailed explanation of the Luma/Chroma weak and strong filtering algorithms directly derived from the C-Model implementation.
- **Visual Influence Ranges**: Clear illustrations showing which pixels are modified and which are used as references during the filtering process.

## Usage

Simply download or clone this repository and open the `cmodel_deblock_dashboard.html` file in any modern web browser. No server or build process is required.

## Contents
- **Global Pipeline Architecture**: Describes the 5-step process from Recon Cache to Output Storage.
- **Boundary Strength Calculation**: Explains the logic for determining BS values.
- **Luma & Chroma Filtering**: Explains the exact C-Model equations and pixel impacts for weak, strong, and VVC long-tap filters.
