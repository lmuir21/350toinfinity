# 350toinfinity

## Project Overview
This repository contains the final project for QTM 350, titled **"Are We Getting Smarter or Just Richer?"**. The project analyzes trends in education enrollment and economic growth across the 15 most populous countries from 2000 to 2022. Using data from the World Bank's World Development Indicators (WDI), we examine the relationship between GDP per capita growth and changes in primary, secondary, and tertiary school enrollment rates.

The repository includes:
- A **[Quarto website](https://lmuir21.github.io/350toinfinity/)** with detailed sections of the analysis.
- A **standalone report** rendered in both [HTML](https://lmuir21.github.io/350toinfinity/analysis_report.html) and [PDF](https://lmuir21.github.io/350toinfinity/analysis_report.pdf) formats.

## How to Run the Code

### Prerequisites
1. Install [Quarto](https://quarto.org/).
2. Ensure you have a working installation of R or Python (depending on the code used in the `.qmd` files).
3. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/lmuir21/350toinfinity.git
   cd 350toinfinity

### Rendering the Website

To render the Quarto website:
1. Open a terminal or command prompt. 
2. Navigate to the directory where you cloned the repository.
3. Run the following command to render the Quarto website:
   ```bash
   quarto render
   ``` 
4. The website will be generated in the docs folder. You can preview it locally by running:
   ```bash
   quarto preview
   ```

### Rendering the Report

To render the standalone report: 
1. Open a terminal or command prompt.
2. Navigate to the directory where you cloned the repository.
3. Run the following command to render the report:
   ```bash
   quarto render analysis_report.qmd --output-dir=docs --output-format=html
   ``` 
4. The report will be generated in the docs folder. You can preview it locally by running:
    ```bash
    quarto preview analysis_report.qmd --output-dir=docs --output-format=html
    ```

### Deployment

Once the website and report are rendered, push the docs folder to your GitHub repository. Configure GitHub Pages to serve content from the docs folder. This will make both the website and the standalone report accessible online.

### Authors
- Daisy Cossio
- Iliyan Sherali
- Liane Muir