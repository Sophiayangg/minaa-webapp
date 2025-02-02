# MiNAA Web App

<img src="www/logo.png" style="width:40%;" align=right>

[![GitHub Releases](https://img.shields.io/github/v/release/solislemuslab/minaa-webapp?display_name=tag)](https://github.com/solislemuslab/minaa-webapp/releases) [![GitHub license](https://img.shields.io/github/license/solislemuslab/minaa-webapp)](https://github.com/solislemuslab/minaa-webapp/blob/main/LICENCE) [![GitHub Issues](https://img.shields.io/github/issues/solislemuslab/minaa-webapp)](https://github.com/solislemuslab/minaa-webapp/issues) ![ ](https://img.shields.io/github/languages/code-size/solislemuslab/minaa-webapp)

## Description

The **MiNAA Web App** is a wrapper around [MiNAA](https://github.com/solislemuslab/minaa) built with R Shiny for the purpose of simplifying and enhancing user interaction with it. When complete, this app will be live at [https://minaa.wid.wisc.edu](/).

**MiNAA** is a standalone program which aligns a pair of given networks on the basis of their topological and biological data. Follow the instructions in [MiNAA's Repository](https://github.com/solislemuslab/minaa) to run MiNAA locally in the terminal.

## Installation and Running Locally

### Prerequisites
Ensure you have the following installed before running the app:

- **R (version 4.0 or later)** – [Download R](https://cran.r-project.org/)
- **RStudio (optional but recommended)** – [Download RStudio](https://posit.co/download/rstudio-desktop/)
- **Git** (for cloning the repository)

### 1. Clone the Repository
Open a terminal or command prompt and run:

```sh
git clone https://github.com/Sophiayangg/minaa-webapp.git
cd minaa-webapp
```

### 2. Compile MiNAA
Before running the Shiny app, you need to compile MiNAA using the Makefile:

```sh
make
```
This step ensures that MiNAA is properly built and ready to be used by the web application.

### 3. Install Dependencies
Before running the application, install the required R packages by executing the following command in RStudio or an R session:

```sh
install.packages(c(
  "shiny", "shinyWidgets", "shinyBS", "shinythemes", "shinycssloaders",
  "colourpicker", "jpeg", "png", "igraph", "plotly", "htmlwidgets", "webshot"
))
```

### 4. Run the Shiny App Locally
Once dependencies are installed, launch the app by running:

```sh
shiny::runApp()
```

### 5. Access the Web App
Once the app starts, it will automatically open in your default web browser at:
`http://127.0.0.1:3838/`

If the app does not open automatically, copy and paste the address into your browser.



## Contributions, Questions, Issues, and Feedback

Users interested in expanding functionalities in the MiNAA Web App are welcome to do so. Issues reports are encouraged through Github's [issue tracker](https://github.com/solislemuslab/minaa-webapp/issues). See details on how to contribute and report issues in [CONTRIBUTING.md](https://github.com/solislemuslab/minaa-webapp/blob/master/CONTRIBUTING.md).

## License

The MiNAA Web App is licensed under the [MIT](https://opensource.org/licenses/MIT) licence. &copy; SolisLemus lab projects (2025)

## Citation

If you use MiNAA in your work, we kindly ask that you cite the following paper:

```bibtex
@ARTICLE{Nelson2022,
  title         = "MiNAA: Microbiome Network Alignment Algorithm",
  author        = "Nelson, Reed and Aghdam, Rosa and
                   Solis-Lemus, Claudia",
  year          =  2022,
  archivePrefix = "arXiv",
  primaryClass  = "q-bio.PE",
  eprint        = "xxx"
}
```

## Acknowledgments

Some components of this web app were inspired by R Studio's [Shiny Examples](https://github.com/rstudio/shiny-examples).
