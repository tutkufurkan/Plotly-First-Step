# Plotly Data Visualization Tutorial

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Plotly](https://img.shields.io/badge/Plotly-Latest-blue.svg)](https://plotly.com/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/sekertutku/Plotly-First-Step)

## Overview

This repository provides a comprehensive tutorial on interactive data visualization using the Plotly library in Python. The project demonstrates 12 distinct visualization techniques through practical examples using the World University Rankings dataset, showcasing Plotly's powerful interactive capabilities for exploring complex relationships in educational data.

## 🎮 Interactive Demo

**👉 [Run the Interactive Notebook on Kaggle](https://www.kaggle.com/code/dandrandandran2093/plotly-first-steps)**

*For the best experience with interactive Plotly visualizations and pre-configured datasets, use the Kaggle notebook above. All visualizations are ready to run with hover, zoom, and pan capabilities!*

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

The analysis utilizes the **World University Rankings** dataset which includes:

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

Additional supplementary datasets:
- CWUR World University Rankings
- Shanghai Rankings
- Educational attainment data
- Education expenditure statistics
- School and country mapping tables

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
numpy>=1.21.0
pandas>=1.3.0
plotly>=5.0.0
jupyter>=1.0.0
wordcloud>=1.8.0
```

## Installation

### Option 1: Use Kaggle (Recommended) ⭐

The easiest way to explore this tutorial is on Kaggle where everything is pre-configured:

👉 **[Open Interactive Notebook on Kaggle](https://www.kaggle.com/code/dandrandandran2093/plotly-first-steps)**

### Option 2: Run Locally

1. Clone the repository:
```bash
git clone https://github.com/sekertutku/Plotly-First-Steps.git
cd Plotly-First-Steps
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. **Datasets:**
   
   ✨ All datasets are included in the `input/` directory for reference:
   ```
   input/
   ├── cwurData.csv
   ├── education_expenditure_supplementary_data.csv
   ├── educational_attainment_supplementary_data.csv
   ├── school_and_country_table.csv
   ├── shanghaiData.csv
   └── timesData.csv
   ```
   
   **Note:** The code uses Kaggle-specific paths (`/kaggle/input/...`). To run locally, update the dataset paths in the code from:
   ```python
   df = pd.read_csv(r"/kaggle/input/dataset-name/file.csv")
   ```
   to:
   ```python
   df = pd.read_csv("input/file.csv")
   ```

## Usage

### On Kaggle (Recommended)

Simply open the [Kaggle notebook](https://www.kaggle.com/code/dandrandandran2093/plotly-first-steps) and run the cells. All dependencies and datasets are pre-configured!

### Locally

Execute the main script to generate all visualizations:

```bash
python plotly-first-steps.py
```

Or run individual sections in a Jupyter notebook environment:

```bash
jupyter notebook plotly-first-steps.ipynb
```

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

### How to Contribute
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the Apache License 2.0 - see the LICENSE file for details.

## References

### Course
- **Udemy**: Data Visualization by DATAI TEAM

### Tutorial
- Kaggle Notebook: [Plotly Tutorial for Beginners](https://www.kaggle.com/code/kanncaa1/plotly-tutorial-for-beginners)

### Documentation
- [Plotly Official Documentation](https://plotly.com/python/)
- [Plotly Graph Objects](https://plotly.com/python/graph-objects/)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [NumPy Documentation](https://numpy.org/doc/)

### Related Projects
- 📊 [Seaborn Data Visualization Tutorial](https://github.com/sekertutku/SeaBorn-First-Steps) | [Kaggle](https://www.kaggle.com/code/dandrandandran2093/seaborn-first-steps)

## Acknowledgments

Special thanks to:
- DATAI TEAM for the comprehensive data visualization course
- Times Higher Education for the World University Rankings dataset
- Plotly team for creating an amazing visualization library
- The open-source community for making these tools accessible

---

**Note**: This tutorial is intended for educational purposes. The interactive features of Plotly are best experienced in Jupyter notebooks or web-based environments like Kaggle.

## 📞 Connect

If you have questions or suggestions:
- Open an issue in this repository
- Connect on [Kaggle](https://www.kaggle.com/dandrandandran2093)
- Star this repository if you found it helpful!

---

**Happy Visualizing! 📊✨**
