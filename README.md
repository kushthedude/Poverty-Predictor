# Combining satellite imagery and machine learning to predict poverty

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/a6d8549100b5440ba30cfbddbc996cd2)](https://app.codacy.com/app/kushthedude/Poverty-Predictor?utm_source=github.com&utm_medium=referral&utm_content=kushthedude/Poverty-Predictor&utm_campaign=Badge_Grade_Dashboard)

 ***Combining satellite imagery and machine learning to produce poverty*** 

Code was written in R 3.2.4 

Users of these data should cite Jean, Burke, et al. (2016). If you find an error or have a question, please submit an issue.

## Description of folders

- **data**: Input and output data stored here
- **figures**: Notebooks used to generate Figs. 3-5
- **scripts**: Scripts used to process data and produce Fig. 1
- **model**: Store parameters for trained convolutional neural network

## Packages required

**R**
- R.utils
- magrittr
- foreign
- raster
- readstata13
- plyr
- RColorBrewer
- sp
- lattice
- ggplot2
- grid
- gridExtra

The user can run the following command to automatically install the R packages
```
install.packages(c('R.utils', 'magrittr', 'foreign', 'raster', 'readstata13', 'plyr', 'RColorBrewer', 'sp', 'lattice', 'ggplot2', 'grid', 'gridExtra'), dependencies = T)
```
**Python**
- NumPy
- Pandas
- SciPy
- scikit-learn
- Seaborn
- Geospatial Data Abstraction Library (GDAL)
- Caffe

Caffe and pycaffe
- See [Caffe Installation](https://github.com/BVLC/caffe/wiki/Installation)

We recommend using the open data science platform [Anaconda](https://www.continuum.io/downloads).



To generate Figure 5, the user needs to run

1. DownloadPublicData.R
2. ProcessSurveyData.R
3. save_survey_data.py
4. get_image_download_locations.py
5. (download images)
6. extract_features.py
7. [Figure 5.ipynb](https://github.com/kushthedude/poverty-predictor/blob/master/figures/Figure%205.ipynb)

Referrence Taken From - :
https://arxiv.org/abs/1510.00098
http://science.sciencemag.org/content/353/6301/790
