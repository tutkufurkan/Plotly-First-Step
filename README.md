# Plotly Data Visualization Tutorial

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Plotly](https://img.shields.io/badge/Plotly-Latest-blue.svg)](https://plotly.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)

## Overview

This repository provides a comprehensive tutorial on interactive data visualization using the Plotly library in Python. The project demonstrates 12 distinct visualization techniques through practical examples using the World University Rankings dataset, showcasing Plotly's powerful interactive capabilities for exploring complex relationships in educational data.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Visualization Types](#visualization-types)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Key Features](#key-features)
- [Contributing](#contributing)
- [References](#references)

## Introduction

Plotly is a powerful Python library for creating interactive, publication-quality graphs and dashboards. Unlike static visualization libraries, Plotly enables dynamic exploration of data through features like hover information, zooming, and panning. This tutorial covers fundamental to advanced visualization techniques, demonstrating how to create engaging and informative data visualizations.

## Dataset

The analysis utilizes the **World University Rankings** dataset (timesData.csv) which includes:

- **World Rank**: Global ranking of universities
- **Teaching**: Teaching quality score
- **Research**: Research output and impact score
- **Citations**: Citation impact score
- **Income**: Financial resources score
- **International**: International diversity score
- **Total Score**: Overall performance score
- **Number of Students**: Student enrollment figures
- **Student-Staff Ratio**: Educational resource allocation metric
- **Year**: Data collection year (2011-2016)

## Visualization Types

The tutorial demonstrates 12 distinct interactive visualization techniques:

### 1. Line Charts
- Time series analysis and trend visualization
- Multiple line comparison with hover information
- Citation and teaching metrics vs world ranking

### 2. Scatter Plots
- Multi-year comparative analysis (2014, 2015, 2016)
- Correlation exploration between variables
- Interactive marker-based visualizations

### 3. Bar Charts
- Grouped bar charts for categorical comparison
- Horizontal bar charts with dual-axis visualization
- Relative and stacked bar configurations
- Citation and teaching metrics for top universities

### 4. Pie Charts
- Proportional distribution visualization
- Student enrollment rate analysis
- Interactive hover with percentage display

### 5. Bubble Charts
- Four-dimensional data representation
- World rank vs teaching score with student count (size) and international score (color)
- Dynamic size and color scaling

### 6. Histogram
- Frequency distribution analysis
- Overlapping histogram comparison across years
- Student-staff ratio distribution analysis

### 7. Word Cloud
- Text-based frequency visualization
- Country mention analysis in university data
- Visual representation of categorical dominance

### 8. Box Plots
- Statistical distribution visualization
- Quartile and outlier detection
- Median, IQR, and whisker representation
- Total score and research metric comparison

### 9. Scatter Matrix Plots
- Multi-variable relationship exploration
- Covariance and correlation analysis
- Research, international, and total score relationships

### 10. Inset Plots
- Multiple plots in single frame
- Detailed focus within broader context
- Teaching and income vs world rank visualization

### 11. 3D Scatter Plots with Colorscaling
- Three-dimensional data exploration
- Fourth dimension through color scaling
- World rank vs research vs citations with teaching score coloring

### 12. Multiple Subplots
- Complex multi-chart layouts
- Simultaneous comparison of multiple metrics
- Research, citations, income, and total score analysis

## Requirements

```
python >= 3.x
numpy>=1.21.0
pandas>=1.3.0
plotly>=5.0.0
matplotlib>=3.4.0
wordcloud>=1.8.0
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/sekertutku/Plotly-First-Steps.git
cd Plotly-First-Steps
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Download the dataset and place it in the `input/` directory.

## Usage

Execute the main script to generate all visualizations:

```bash
python plotly-first-steps.py
```

Or run individual sections in a Jupyter notebook environment:

```bash
jupyter notebook plotly-first-steps.ipynb
```

## 🎮 Interactive Demo

Experience the full interactive visualizations on Kaggle:  
👉 [Try Interactive Plotly Tutorial](https://www.kaggle.com/code/SENIN-USERNAME/plotly-first-steps)

*Note: Plotly's interactive features (hover, zoom, pan) work best in Kaggle's environment.*

## Key Features

### Interactive Capabilities
- **Hover Information**: Detailed data points on mouse hover
- **Zoom & Pan**: Dynamic exploration of data regions
- **Toggle Traces**: Show/hide specific data series
- **Responsive Design**: Adapts to different screen sizes

### Advanced Visualizations
- **Multi-dimensional Analysis**: Color, size, and position encoding
- **Statistical Distributions**: Box plots with quartile information
- **3D Visualization**: Three-dimensional scatter plots with rotation
- **Subplot Layouts**: Complex multi-chart arrangements

### Customization Options
- **Color Schemes**: RGB, RGBA, and named color palettes
- **Marker Styles**: Size, opacity, and border customization
- **Layout Control**: Title, axis labels, and legend positioning
- **Annotation Support**: Text labels and highlighting

## Key Insights

The analysis reveals important patterns in global university rankings:

- **Research-Citation Correlation**: Strong positive relationship between research output and citation impact
- **Teaching Quality Trends**: Top-ranked universities maintain consistently high teaching scores
- **International Diversity**: Significant variation in international student representation across institutions
- **Resource Allocation**: Student-staff ratio impacts overall university performance
- **Temporal Stability**: Top universities maintain rankings across multiple years
- **Geographic Patterns**: Certain countries dominate top-tier university rankings

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss proposed modifications.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## References

- Udemy Course: Data Visualization by DATAI TEAM
- Kaggle Notebook: [Plotly Tutorial for Beginners](https://www.kaggle.com/code/kanncaa1/plotly-tutorial-for-beginners)
- [Plotly Official Documentation](https://plotly.com/python/)
- [Plotly Graph Objects](https://plotly.com/python/graph-objects/)

## Acknowledgments

Special thanks to the Times Higher Education World University Rankings for providing the dataset and to the open-source community for making these visualization tools accessible.

---

**Note**: This tutorial is intended for educational purposes. The interactive features of Plotly are best experienced in Jupyter notebooks or web-based environments.
