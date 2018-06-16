# Setting up R and RStudio in Windows

## Running as Administrator

- When you run the installers, make sure to run them as administrator.
- Select the file, right click and choose **Run as administrator**  
  <img src="Figures/admin_run.png" alt="" style="width: 150"/>

## Installing R

- Open your browser and go to http://cran.r-project.org/
- Click on `Download R for Windows`  
  <img src="Figures/cran01.png" alt="" style="width: 400"/>
- Click on `base`  
  <img src="Figures/cran02.png" alt="" style="width: 400"/>
- Click on `Download R 3.1.2 for Windows`  
  <img src="Figures/cran03.png" alt="" style="width: 400"/>
- Open and run the file you just downloaded `R-3.1.2-win.exe`
  <img src="Figures/install_r01.png" width="40"/>
- There is no need to change the default installation!

|                            .                            |                            .                            |                            .                            |
| :-----------------------------------------------------: | :-----------------------------------------------------: | :-----------------------------------------------------: |
| <img src="Figures/install_r02.png" alt="" width="250"/> | <img src="Figures/install_r03.png" alt="" width="250"/> | <img src="Figures/install_r04.png" alt="" width="250"/> |
|                          **1**                          |                          **2**                          |                          **3**                          |
| <img src="Figures/install_r05.png" alt="" width="250"/> | <img src="Figures/install_r06.png" alt="" width="250"/> | <img src="Figures/install_r07.png" alt="" width="250"/> |
|                          **4**                          |                          **5**                          |                          **6**                          |
| <img src="Figures/install_r08.png" alt="" width="250"/> | <img src="Figures/install_r09.png" alt="" width="250"/> | <img src="Figures/install_r10.png" alt="" width="250"/> |
|                          **7**                          |                          **8**                          |                          **9**                          |
| <img src="Figures/install_r11.png" alt="" width="250"/> | <img src="Figures/install_r12.png" alt="" width="250"/> |                        **DONE**                         |
|                         **10**                          |                         **11**                          |                                                         |

- Please make sure you install the latest version of R (R version 3.1.2).

## Installing Rtools

Now we need to install Rtools

- Open your browser and go to http://cran.r-project.org/
- Click on `Download R for Windows`  
  <img src="Figures/cran01.png" alt="" width="400"/>
- Click on `Rtools`  
  <img src="Figures/rtools00.png" alt="" width="400"/>
- Download `Rtools31.exe`  
  <img src="Figures/rtools01.png" alt="" width="400"/>
- Open and run the file you just downloaded `Rtools31.exe`
  <img src="Figures/rtools02.png" alt="" width="40"/>
- Again, there is no need to change the defaults

|                          .                           |                          .                           |                          .                           |
| :--------------------------------------------------: | :--------------------------------------------------: | :--------------------------------------------------: |
| <img src="Figures/rtools03.png" alt="" width="250"/> | <img src="Figures/rtools04.png" alt="" width="250"/> | <img src="Figures/rtools05.png" alt="" width="250"/> |
|                        **1**                         |                        **2**                         |                        **3**                         |
| <img src="Figures/rtools06.png" alt="" width="250"/> | <img src="Figures/rtools07.png" alt="" width="250"/> | <img src="Figures/rtools08.png" alt="" width="250"/> |
|                        **4**                         |                        **5**                         |                        **6**                         |
| <img src="Figures/rtools09.png" alt="" width="250"/> | <img src="Figures/rtools10.png" alt="" width="250"/> | <img src="Figures/rtools11.png" alt="" width="250"/> |
|                        **7**                         |                        **8**                         |                        **9**                         |
| <img src="Figures/rtools12.png" alt="" width="250"/> | <img src="Figures/rtools13.png" alt="" width="250"/> | <img src="Figures/rtools14.png" alt="" width="250"/> |
|                        **10**                        |                        **11**                        |                        **12**                        |
| <img src="Figures/rtools15.png" alt="" width="250"/> |                       **DONE**                       |                                                      |
|                        **13**                        |                        **14**                        |                                                      |

## Installing RStudio

- If you have already installed RStudio, before you skip this section check if you are using the right R version. Go to `Tools/Global Options`. Make you sure you have `R-3.1.2` under R version

<img src="Figures/rstudio10.png" alt="" width="400"/>

- Go to http://www.rstudio.com/ and click on `Desktop`

<img src="Figures/rstudio01.png" alt="" width="400"/>

- Select `DOWNLOAD RSTUDIO DESKTOP`

<img src="Figures/rstudio02.png" alt="" width="400"/>

- Download the installer for Windows

<img src="Figures/rstudio03.png" alt="" width="400"/>

- Open and run the file you just downloaded `RStudio-0.98.1091.exe`

<img src="Figures/rstudio04.png" alt="" width="40"/>

- You don't have to change any of the defaults for the installation

|                           .                           |                           .                           |                           .                           |
| :---------------------------------------------------: | :---------------------------------------------------: | :---------------------------------------------------: |
| <img src="Figures/rstudio05.png" alt="" width="250"/> | <img src="Figures/rstudio06.png" alt="" width="250"/> | <img src="Figures/rstudio07.png" alt="" width="250"/> |
|                         **1**                         |                         **2**                         |                         **3**                         |
| <img src="Figures/rstudio08.png" alt="" width="250"/> | <img src="Figures/rstudio09.png" alt="" width="250"/> |                       **DONE**                        |
|                         **4**                         |                         **5**                         |                         **6**                         |

## Installing devtools

- Open Rstudio, in the **Files/Plots/Packages/Help** panel, select **Packages** and then click on **Install**
  <img src="Figures/devtools01.png" alt="" width="400"/>

- Type `devtools` under **Packages**, make sure you spell the name of the package correctly. Then, click on **Install**  
  <img src="Figures/devtools02.png" alt="" width="400"/>

- Alternatively, you can run the following command in the console:

```
install.packages("devtools")
```

## Installing packages from GitHub

We are ready to install R packages from GitHub

- First we need to load the `devtools` package

```r
library(devtools)
```

- Now we can install the `gapminder` package.

```r
install_github("jennybc/gapminder")
```

## License

http://opensource.org/licenses/MIT
