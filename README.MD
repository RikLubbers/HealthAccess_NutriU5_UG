<div align="center">
    <h1>Physical Accessibility to Public Healthcare Facilities and Undernutrition in Children Under 5 in Uganda</h1>
</div>

## Description

This repository contains the code for the first study of my PhD research in the Global Health Unit at the University Medical Center Groningen (UMCG). Study 1 is an analysis of the impact of physical accessibility on undernutrition outcomes in children under-5 in Uganda.

## Table of Contents

- [Study Title](#physical-accessibility-to-public-healthcare-facilities-and-undernutrition-in-children-under-5-in-uganda)
  - [Description](#description)
  - [Table of Contents](#table-of-contents)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
  - [Usage](#usage)
  - [Contributing](#contributing)
  - [License](#license)

## Getting Started

### Prerequisites

#### Software
- [R](https://www.r-project.org/) (version 4.0.3 or higher)
- [RStudio](https://rstudio.com/) (version 1.4.1106 or higher) or any other IDE for R
- [Git](https://git-scm.com/) (version 2.30.0 or higher)
- [GitHub Desktop](https://desktop.github.com/) (version 2.6.3 or higher) or any other Git client
- [ARC-GIS](https://www.arcgis.com/index.html) (version 10.8.1 or higher) or any other GIS software
- [Access Mod 5](https://www.accessmod.org/) (version 5.0.0 or higher)

#### R packages
The code is written in R and requires multiple packages. They are listed below:

    ```r
    # List of required packages
    library(NCmisc)
    library(tidyverse)
    library(haven)
    library(lattice)
    library(data.table)
    library(knitr)
    library(survey)
        options(survey.lonely.psu = "adjust")
    library(expss)
    library(labelled)
    library(table1)
    library(readxl)
    library(GGally)
    library(kableExtra)
    library(xtable)
    library(modelsummary)
    library(performance)
    library(finalfit)
    library(naniar)
    library(rms)
    library(openxlsx)
    library(rcompanion)
    library(questionr)
    library(flextable)
    library(MASS)
    library(car)
    library(cowplot)
    library(heatmaply)
    library(esquisse)
    library(visreg)
    library(forcats)
    library(mosaic)
    library(DT)
    library(mice)
    library(gtsummary)
    library(styler)
    library(languageserver)
    library(httpgd)
    ```

## Usage

To run the code in this repository, you will need to install the software above and download the code and data. The following sections explain how to do this.:

### Downloading the code and data

To download the code and data in this repository, you can either:

- Clone the repository using Git
- Download the repository as a ZIP file by clicking on the green "Code" button on the repository homepage and selecting "Download ZIP"

Once you have downloaded the repository, you can open the R project file (`PhD-Code.Rproj`) in RStudio and run the code in the various R scripts.

Note that not all the data used in this study is publicly available due to licensing. For an overview of all the datasets see [here](https://github.com/RikLubbers/PhD-Code/blob/main/Study_1/DATA/Data_overview.md). The data that is publicly available can be downloaded from the links provided in the file. The data that is not publicly available can be requested from the respective sources as listed.

#### Important Note on AccessMod
It's essential to mention that the usage of AccessMod in this project does not allow for a fully reproducible workflow. AccessMod is an external tool that requires manual input and customization based on data. While the code provided can reproduce the models given the travel time data, the travel time data itself cannot be reproduced without manual input.

## Contributing

You are welcome to contribute to this project by submitting bug reports, suggesting improvements, or sending pull requests. However, it is advisable to first contact the project owner, Rik Lubbers, at [r.u.lubbers@rug.nl](mailto:r.u.lubbers@rug.nl) or [r.u.lubbers@umcg.nl](mailto:r.u.lubbers@umcg.nl) to discuss your ideas or changes before making any contributions. Please feel free to contribute to the discussion board as well.

Your contributions are highly appreciated and can help make this project better. Please follow the guidelines and best practices for contributing outlined in the [CONTRIBUTING.md](https://github.com/RikLubbers/PhD-Code/blob/main/CONTRIBUTING.md) file.

## License

Please refer to the [LICENSE.txt](https://github.com/RikLubbers/PhD-Code/blob/main/LICENSE.txt) file in the top directory for details.

---
