# Generalized Linear Models in R

Coursework project exploring two generalized linear models (GLMs) using R: a **binomial logistic regression** for university transportation choices and a **Poisson regression** for heart-beat counts under different exercise routines.

## Analyses

1. **University transportation:** Models use of a private vehicle as a function of distance, age, and sex. Includes logit-linearity checks, variance inflation factors, a Hosmer–Lemeshow test, influence diagnostics, sensitivity analysis, and predicted probabilities.
2. **Heart-beat counts:** Models recorded beats by treatment/routine, height, and habitual exercise. Includes checks of the log-link functional form, dispersion, influence diagnostics, sensitivity analysis, and predicted counts.

The original report includes the interpretation of estimates and limitations, including influential observations and underdispersion in the Poisson analysis. These are course exercises, not published epidemiological research.

## Files

- `analysis/Taller5.Rmd`: complete analysis and discussion (Spanish), with data paths adjusted for this repository.
- `data/datos.xlsx`: workbook used by both exercises, with worksheets `Ejercicio_1` and `Ejercicio_2`.

## Reproducing the analysis

1. Open R or RStudio and set the working directory to the repository root.
2. Install the required packages:

   ```r
   install.packages(c("rmarkdown", "readxl", "car", "ResourceSelection", "ggeffects", "ggplot2", "scales"))
   ```
3. Render from the repository root:

   ```r
   rmarkdown::render("analysis/Taller5.Rmd", output_dir = "output")
   ```

The original R Markdown requests PDF output with XeLaTeX; a compatible LaTeX installation is required. The document contains LaTeX-specific formatting and was not independently rendered as part of this repository preparation.

## Credits

Original coursework: **Juanita Guerrero and María José Camacho** (Group 6, *Biología Cuantitativa*, Universidad de los Andes). The report retains its original shared authorship. Repository organization and documentation are for portfolio presentation.
