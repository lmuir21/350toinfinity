# 350toinfinity

## Project Overview
This repository contains the final project for QTM 350: **"Are We Getting Smarter or Just Richer? A Global Analysis of Education Enrollment and Economic Growth (2000-2022)"**. The project analyzes trends in education development and economic growth across the 15 most populous countries in the world from 2000 to 2022. Using data from the World Bank's World Development Indicators (WDI), we examine the relationship between GDP per capita growth and changes in primary, secondary, and tertiary school enrollment rates.

The repository includes:
- A **[Quarto website](https://lmuir21.github.io/350toinfinity/)** with detailed sections of the analysis.
- A **standalone report** rendered in both [HTML](https://lmuir21.github.io/350toinfinity/analysis_report.html) and [PDF](https://lmuir21.github.io/350toinfinity/analysis_report.pdf) formats.
- Python and SQL scripts for data cleaning and analysis.
- The cleaned dataset (`epi_top15.csv`) used for the analysis.
- An accompanying codebook (`codebook.md`) located in the `documentation` folder, describing the dataset's variables and structure.

---

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

To deploy the website and report:

1. Push the docs folder to your GitHub repository:
    ```bash
    git add .
    git commit -m "Add rendered website and report"
    git push origin main
    ```
2. Ensure that GitHub Pages is enabled for the `docs` folder in your repository settings.
3. The website will be available at `https://<your-username>.github.io/350toinfinity/`.
4. The report will be available at `https://<your-username>.github.io/350toinfinity/analysis_report.html`.
5. You can also download the PDF report directly from the `docs` folder.

### License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

### Acknowledgments
This project was completed as part of the QTM 350 course at Emory University. Special thanks to our instructor Prof. Freire for teaching this course and to TAs Alex and Harris for their invaluable guidance throughout the semester. 

### Authors
- Daisy Cossio
- Iliyan Sherali
- Liane Muir

