<p align="center">
 <img src="https://i.imgur.com/rSyq3MW.png" alt="The Documentation Compendium"></a>
</p>

<h3 align="center">The Documentation </h3>

<div align="center">

<!--   <a href="https://www.producthunt.com/posts/the-documentation-compendium?utm_source=badge-top-post-badge&utm_medium=badge&utm_souce=badge-the-documentation-compendium" target="_blank"><img src="https://api.producthunt.com/widgets/embed-image/v1/top-post-badge.svg?post_id=157965&theme=dark&period=daily" alt="The Documentation Compendium - Beautiful README templates that people want to read. | Product Hunt Embed" style="width: 250px; height: 54px;" width="250px" height="54px" /></a> -->

</div>

---

<p align = "center">💡 implementing Time Series NBEAT algoritm with RIVIN over 50 dataset given.</p>


## Table of Contents


- [Libraries Used](#best_practices)
- [Repository use](#templates)
  - [Google Colab](#google_colab)
  - [Local (Windows Machine)](#local)
  - [Runnning perticular File First](#first)

- [References](#acknowledgements)



## Libraries Used/Required<a name = "best_practices"></a>
```
   Python  3.7 or higher
   Tensorflow (GPU is prefered)
   Pytorch 
   csv
   numpy
   os
   Pandas 
   Matplotlib
```
**Things to remember:**


## Repository <a name = "templates"></a>
*   There are 2 files one for running the scrpit over google colab named ```NBEATS_Colab.ipynb``` 
another one ```NBEATS_windows.ipynb``` to run locally over windows machine
*   The scipt is writtern in Jupyter Notebook ```ipynb``` 
*   The Code plots the CSV data in a file ```temp.csv```
*   The scrpit saves the plot shown in the folder in ```content``

## Google Colab(NBEATS_Colab) <a name = "google_colab"></a>
### The whole code is one touch go in colab no need to download or setup files
### you just need to run the instance again and again to cycle through files from 0-49.csv
*   When The Whole code is Run once the plots are visible and files are stores in machine instance
    *   The scripts is written in way that can be run over google colab without downloading the files
     (there are built in scripts that download the files and shows and saves the plots file over running instance machine on google colab)
    *   The code when run once shows the various plots in the insstance which on time of initialisation starts with ```0.csv```and saves the plot
    at online machine instance in ```content``` folder 
    *   The  ```MAE, MSE, RMSE, MAPE, MASE``` value of the file are saved in temp.csv file with the first number indicating file index number
     in the same ```content```     folder
    *   When the whole script is run  the code now moves to the next file then shows and saves the next file PLOT and ```append``` the metrics data over ```temp.csv```
    file
* when the code is run once more it moves onto the next csv data and saves its data in the files 
    ** for example -> csv 
## Local (Windows Machine) <a name = "local"></a>
### the file is different named(NBEATS_window) to be run on local machine
### There are some steps to setup
  1. First ensure [libraries](#best_practices) are installed in you enviornment on which you are gonna run
  2. Create folder named ```content``` in the same directory as the path of code 
  3. put all the CSv data file from 0-49.csv in ```content``` folder
  4. create two empty CSV file inside ```content```folder  named ```-1.csv``` and ```temp.csv```
    * (alternatively) you can download https://github.com/tambeanuj123/tambeanuj123/blob/main/dataset50/temp.csv ```and``` https://github.com/tambeanuj123/tambeanuj123/blob/main/dataset50/temp.csv files and put them in ```content``` folder
### Now you can open the file and run an instance 
*   running the instance once will show you plot of the data 
*   the plots are saved as png file with the files corresponding name such as ```img1_first.png``` , ```img1_prediction.png``` ,  ```img_full_prediction.png```
*   The temp.csv file gets appended  index of file  and ```MAE, MSE, RMSE, MAPE, MASE``` of the prediction values in the same order
### once instance is completed the process is repeated for next index.csv file in loop and data is saved


## Running perticular file first <a name = "first"></a>
### just go to the notebook and  find
- ```filecount=0 ```      # change this value to the index of file you want to run first
- **NOTE** keep this in mind this will only work for the first instance if you want to reset this clear the ```temp.csv``` in folder ```contents```


](https://drive.google.com/drive/folders/13ifIVRwStWzRVUqhKVWwwa2-NNTE3hb2?usp=sharing)

## References <a name = "acknowledgements"></a>

NBEATS official implementation: [https://github.com/ElementAI/N-BEATS](https://github.com/ElementAI/N-BEATS)

NBEATS paper: [https://arxiv.org/abs/1905.10437](https://arxiv.org/abs/1905.10437)

RIVIN paper: [https://openreview.net/pdf?id=cGDAkQo1C0p](https://openreview.net/pdf?id=cGDAkQo1C0p)
dataset link: [https://drive.google.com/drive/folders/13ifIVRwStWzRVUqhKVWwwa2-NNTE3hb2?usp=sharing](https://drive.google.com/drive/folders/13ifIVRwStWzRVUqhKVWwwa2-NNTE3hb2?usp=sharing)


