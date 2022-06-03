# Lostlifevalue
# 1 .Dataset
Population: https://www.worldometers.info/world-population/population-by-country/ <br>
VSL,GNI: https://law.vanderbilt.edu/phd/faculty/w-kip-viscusi/355_Income_Elasticities_and_Global_VSL.pdf <br>
deaths: https://github.com/owid/covid-19-data/blob/master/public/data/jhu/total_deaths.csv <br>
# 2. Package
This package is designed to calculate the value of lives lost due to Covid-19 and to determine how much damage the country has suffered in terms of GNI ratio.<br>
To calculate the value of a life, we use an index called VSL. This index stands for value of statistical life, and represents the value of a human life. Using this VSL data and the number of deaths due to Covid-19, we can calculate the value of lives lost due to Covid-19.<br>
The following indicators are used in this package.<br>
deaths<br>
VSL ($/million)<br>
GNI ($/thousand)<br>
Population(/100000)<br>
eloss_total(VSL * deaths)<br>
GNI_total(GNI * Population)<br>
eDamage_per_GNI(eloss_total/GNI_total)<br>
# 3. How to rum?
You can use this package easily.<br>
First, use this command to download the package.<br>
$ pip install lostlifevalue<br>
Next, run this command.<br>
$ lostlifevalue Items_to_be_sorted<br>
When you run the above command, you will be asked a question like the one in the image.<br>
![スクリーンショット 2022-01-26 19 21 14](https://user-images.githubusercontent.com/60126632/151146228-6237ed9e-f5a2-4535-b384-6f90018a2efb.png)<br>
This will ask you which value you want to sort the table by, so follow the instructions and enter your choice of deaths, VSL, or eDamage_per_GNI.<br>
![スクリーンショット 2022-01-12 1 18 05](https://user-images.githubusercontent.com/60126632/148980554-10890f88-65ce-445b-84c8-88bf588ef59f.png)
