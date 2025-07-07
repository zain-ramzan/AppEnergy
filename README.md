# AppEnergy: Software Application Energy Consumption Calculator

## Overview

**AppEnergy is a specialized Python package designed to analyze software applications and determine their estimated energy consumption levels**. It functions as an **energy consumption calculator for software applications**. The core functionality involves **fetching application data from a variety of sources**, including Snapcraft, Flathub, Apple Store, GOG, Itch.io, and MyAbandonware. This data is then processed using **intelligent matching algorithms to identify energy usage patterns**, providing insights into an application's CPU intensity.

## Features

AppEnergy offers a robust set of features to facilitate energy consumption assessment:

*   **Multi-source Data Fetching**: The tool gathers comprehensive application information from **over 5 distinct sources**.
*   **Intelligent Tag Normalization**: It cleans and **standardizes tags and metadata from various disparate sources**, ensuring consistency for analysis.
*   **Category Matching**: AppEnergy employs **fuzzy matching algorithms with confidence scoring** to accurately categorize applications.
*   **Energy Level Classification**: Applications are systematically categorized into one of three distinct energy profiles: **low-cpu, moderate-cpu, or high-cpu**.
*   **Command Line Interface (CLI)**: A **simple and intuitive command-line interface** is provided for quick energy assessments directly from your terminal.
*   **Python API**: For developers and integrators, AppEnergy offers a **programmatic Python API**, allowing seamless integration into other projects and workflows.

## Installation

Getting started with AppEnergy is straightforward. You can **install the package using pip**:

```bash
pip install AppEnergy
```

## Quick Start & Usage

AppEnergy can be utilized through both its command-line interface and its Python API.

### Command Line Interface (CLI) Usage

For quick assessments, simply run `AppEnergy` followed by the application name.

*   **Single-word applications**:
    ```bash
    AppEnergy Facebook
    # Output: low-energy
    ```
*   **Multi-word applications**:
    (Remember to enclose multi-word names in quotes)
    ```bash
    AppEnergy 'Google Chrome'
    # Output: moderate-cpu
    ```
<!---
### Python API Usage

For programmatic integration into your Python projects, use the `calculate_energy_consumption` function:

```python
from energyscan import calculate_energy_consumption

# Calculate energy level for a specific application
energy_level = calculate_energy_consumption("Chrome")

# Print the result
print(energy_level)
```
--->
## How It Works

AppEnergy's analysis is rooted in its ability to **fetch diverse application data from multiple sources**, including Snapcraft, Flathub, Apple Store, GOG, Itch.io, and MyAbandonware. It then applies **intelligent matching algorithms** to discern energy usage patterns. The system's **category matching** utilizes fuzzy matching with confidence scoring to accurately classify applications. Based on its analysis, AppEnergy performs **energy level classification**, categorizing applications into **low-cpu, moderate-cpu, or high-cpu**, providing a clear indication of their expected CPU intensity and, by extension, their energy consumption. The project is **developed entirely in Python**.

## About the Project

This project aims to provide a valuable tool for understanding the energy footprint of software applications. AppEnergy is a **public repository** and offers a robust foundation for future development and contributions.

***
