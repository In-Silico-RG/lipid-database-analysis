# Lipid Database Analysis and Search System

## Overview
This project provides a comprehensive chemical informatics toolkit for analyzing and searching lipid structures from the LIPID MAPS database. It enables researchers to perform sophisticated queries, visualize chemical space, and export lipid data for further analysis.

## Features
- **Multiple Search Methods**: Name/ID, category/classification, property ranges, structural (SMARTS), and similarity searching.
- **Interactive Interface**: User-friendly command-line interface for exploring lipid data.
- **Chemical Visualization**: Molecular structure display and chemical space analysis.
- **Data Export**: Save results in CSV and SDF formats.

## Installation
1. Clone this repository: `git clone https://github.com/your-username/lipid-database-analysis.git`
2. Install the required Python packages: `pip install rdkit-pypi pandas matplotlib seaborn`

## Usage
```python
# Initialize and load the lipid database
lipid_searcher = LipidMapsSearcher("LMSD.sdf/structures.sdf")
success = lipid_searcher.load_lipid_database()

# Start interactive search
search_engine = EnhancedLipidSearchEngine(lipid_searcher.df)
enhanced_interactive_search(search_engine)

