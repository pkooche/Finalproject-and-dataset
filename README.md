# Finalproject-and-dataset
This repository I about hot to visualize the data set with 2 method 1)gnuplot 2)Rprogramming

First I will discuss about gnuplot In this method first we should run the docker for using ubuntu command in our system , to running a ubuntu in our system fist we should write the command “docker image” to see did we have ubuntu or not ———>if we don’t have ubuntu first we should dl ubuntu with “docker pull ubuntu:14.04” after that we should run the new bash on that specific ubuntu so we use “ docker run -I -t ‘ IMAGE ID’ /bin/bash ———> I few have ubuntu 14.04 we start that “ docker start CONTAINER ID ‘“

After starting the new container we should attach that container to can write our common and excuse them so we should write “ docker attach CONTAINER ID “

After running this command we need our Dataset , to have the data set in our get hb we should do the following steps

Download and install git #sudo apt-get update #sudo apt-get install git


Download local copy of GitHub repository # git clone https://github.com/pkooche/DATASET-


Change into GitHub repository an create folder that we want # cd Finalproject #mkdir Dataset-contain


Copy dates into new data folder (for copy our changes into get hub we should exit from root ) # exit # docker cp “where the file located in our computer “ “the file that we want to have it in our GitHub” ‘ as an example —> docker cp /Users/panteakoochemeshkian/Downloads/gnuplot_tutorial/DATASET.csv 4f14e6cd87a1:/Finalproject/Dataset_contain/DATASET.csv


Make the changes in GitHub repository (online) # git add . #git commit -am “uploading data” ****** if u run this command the the first time in your system you should introduce your self to the system for this action we do ——> # git config - -global user.email “ your email in GitHub” # git config - -global user.name “ your user name in GitHub” After u introduce your self to the system you should run the last command one more time and if you know sure that is your first time you can introduce your self then run the “ git commit -am “uploading data “ “ command . *******Now you can have your data set in your GitHub ***** By this method I provide another folder for gnuplot , to visualize my dataset with gnuplot command For running the gnuplot commands first we should make the directory that we want to save our plot on that , my directory is “gnuplot”, in this folder we have 4 grpah , Figure1 , Figure2 , Figure 3 and the simple.1 the Figure1 present the graph of sin(x) , Figure2 is shown the average monthly houre , the figure 3 shown the realation between average monthly hour and the satisfaction level cause the data set have a lotf data , the figure is not so clear , for having the clear and understandable figure we can bound the data. 



R prgoramming 
 I don't have any graphs in my directory Rprgoramming beacouse i write my code in the online commander, and it's not possible to save the grapgh but i try to figure out how to save it and if i want i will update my file 
 for having a grapgh in R , I try to use the http://localhost/rstudio ,
 I use the below command to drow my ghrapghs :
 
 
 HISTOGRAM GRAPGH in R 
 hist(y[,4], main = "histogram plot of average monthly hours" , xlab="satisfactionlevel", ylab = "monthly average", col = “lightyellow").  ------------> this command means to dry the coloumn 4 of the data set that the avaregae monthly hours and the main show the titile the graphs , ylab an xlab shows the label of x an y for having the colorful grapghs u can also add the command col="the color that you want".
 
 
 
 SCATTER PLOT in R : 
 
scatter.smooth(y[,4],y[,1], xlab ="satisfaction level", ylab = "average monthly hours")

to have the plot wiht two varialbe of the data set we should use the scatter.smooth command 
y[,4] ------> show the 4th coloumn of the data set 
y[,1] ------> show the 1st coloumn of the data set 
*** you can use what coloumn you want to draw the plot 
xlab and ylab show the name the x and y 
to have the clear plot we should name all the varialbe that we use in our command to people who don.t know about the data set by seeing at the plot understad what hte plot shows . 
 
 
 
 
