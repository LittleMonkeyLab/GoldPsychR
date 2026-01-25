# Slide text copied here​

Open Excel file named Lab 12 data​

​

Data is similar to that from seminar 8​

​

What can you see from this data?

---

How many participants are there?​

60​

​

Are all the participants doing exactly the same?​

No – the experimental condition varies​

​

What can we learn about each participant?​

Scores in each condition​

How this changes between conditions​

​

---

What would be the appropriate descriptives?​

​

Mean scores for:​

Baseline​

Control​

Experimental​

​

Also separate means for happy and scary conditions​

​

What do these suggest?​

___

Clearest way to review data is to create a plot​

​

What type of plot would be suitable for this?​

Line graph showing changes over conditions​

​

How many lines?​

1 – just to show change over three conditions​

2 – showing change separately for two experimental conditions​

​

Create a simple line graph in excel showing the change across the 3 conditions​

---

# Lab Activity instructions

Open R and import dataset​

​

Answer the questions on the Data Skills sheet​

​

Upload this to the submission link​

__-

THIS WAS GIVEN AS OPEN DOC FORMAT - DATASKILLS 12 - for submission.

Open R and import lab 12 data. Answer the four questions below, and submit this to the submission link.

Calculate the mean for baseline, control and experimental. Copy and paste the code here, and the results.










Calculate the mean for baseline, control and experiment, separated by condition (1=happy, 2=scary). Copy and paste the code here, and the results.











Plot a line graph showing the first set of means – copy and paste here.











Plot a line graph with 2 lines (one for each condition on the same graph) – copy and paste here.


---

THIS WAS PROVIDED AS R script and students copied and pasted the code and responses into it.

#Week 12 Data Skills

#This is a script for the R programming language
#You can think of it as a list of instructions for computer in a language called R
#You can run the code in a few ways:
#1: line by line by placing your cursor at the start of the line and pressing the green 'Run' button 
#   in the top right of this script, that line of code will be run and the cursor will
#   move to the start next line
#2: You can highlight multiple lines and press the run button to run all of them
#
#Whichever you choose you will notice that those lines of code the appear in the 'console' panel below this script
#This is because running a line of code in a script is exactly the same as typing it out in the console and 
#pressing the 'ENTER' key on your keyboard.

#Lines of text in this document that start with the # symbol are called comments
#These lines will not be executed but are there to explain things 

#IMPORT DATA####
#NOTE By adding the 4 # after the comment it creates what is called a code section
#     You can quickly navigate between sections using the dropdown buttons in the
#     Bottom left of this script

#The first stage is to import the data (please see the video on the VLE for help)
#If you use the 'Import Dataset' button (which can be found in the banner at top of the Environment panel), the 'From Excel...' 
#It will import the data but also show you the code that it used to do this (I've copied the code that works below)

library(readxl) #This command loads a package called 'readxl' that contains the function we need to read excel files
#R has a certain set of functions in what is called it's 'base' package
#Packages are extra sets of functions that R can use to do other things
#Many packages will already be installed as part of R Studio
#If a package is installed we need to tell R to load those functions into its memory

Lab_12_data <- read_excel("Lab 12 data.xlsx") #this command loads the data and gives the data set the name Lab_12_data
#this data is a type of data called a dataframe, this is like a spreadsheet with multiple rows (one for each participant in the experiment),
#and multiple columns, that contain different things that were measured about that participant
#each column can have a different type of data (column 1 might be text and column 2 might be numbers)
#in this case all columns have numbers in them
#NOTE: technically this is a special type of dataframe called a tibble but we will cover that late in the term

View(Lab_12_data) #this command opens the data set in the variable viewer, you can also do this by double clicking on the data set in the Environment panel
#View() is what is called a function, it takes an input (the thing inside the brackets) and does something with it

#In this dataset each participant took part in three conditions called 'Base', 'Control', and 'Expt'. For each condition they did three trials of that type
#For example Base trial 1 is the column Base1 and trial 2 in the Control condition is called Control2, etc.

#ACCESSING DATA####
#to access a specific column in a data frame we can use multiple options in R
#the easiest is to use the $ sign to get the column by name e.g.
Lab_12_data$Base1
#We could also access columns by their number
Lab_12_data[,3]
#to access data in a dataframe like this in R we use square brackets []
#if we wanted to access a single bit of data we would use
Lab_12_data[1,3]
#this command would get us the piece of data in the first row of the third column
#You may be familiar with similar ways of accessing data in excel
#if instead we want a whole column we leave the bit before the comma blank
Lab_12_data[,3]
#we can also access the third row of the data by putting a 3 before the comma and leaving the bit afterwards blank
Lab_12_data[3,]
#Accessing data in this way is often referred to as indexing (like the index in a book)


#TASK 1####

#Calculate the mean for baseline, control and experimental. Copy and paste the code here, and the results.

#if we want to get the mean of a single column we need a function that does this for us
#In R the function is called mean()
#Before using a function we should always check the documentation to understand how to use it properly
#we do this using the help() function
help(mean) #this will display the help in the bottom right panel of RStudio
#The help sections in R can sometimes look very complicated, the main thing we need to know is what order the inputs go in
#The examples at the bottom are often a good place to start.
#In this case we only need one input which is our data:
mean(Lab_12_data$Base1) #produces the mean of the Base1 column in Lab_12_data
#If you run the line of code above it will print the mean of that column in the console (Bottom left of RStudio)
#However, if you look in the environment panel (top right of RStudio) no new variable has been created to store the result
#Normally we want to store things we calculate, to do this we need to assign the output of the function to a new variable
myBase1Mean <- mean(Lab_12_data$Base1)
#If you run the previous line you will see that it now creates a new variable called myBase1Mean which stores our value
#We use the <- symbols to assign data to a variable in R, you can also use = but for reasons we won't go into here <- is 
#more commonly used so please try to stick to that.

#We could calculate the mean of each column this way but it involves a lot of typing and creating multiple variables
#When trying to write code it is generally better to avoid doing this
#Helpfully there is a function that can calculate the means of all of our columns in one go called colMeans()
myColumnMeans <- colMeans(Lab_12_data)
#it might be tempting to call our new variable colMeans but it is important to never give a variable the same name as an existing function
#If you do then R doesn't know whether you are referring to the variable or the function later on

#We now need to average the data for the 3 trials in each condition so we end up with the overall mean for baseline, control, and experimental
#We can use the square brackets [] to get bits of data out of our myColumnMeans variable
#The 3 columns for the baseline condition were numbers 3,4, and 5, in R we can use the : to get a list of numbers between two numbers
#for example 
2:8
#If you run the line above it will print the numbers 2,3,4,5,6,7, and 8 to the command window
#so the line below with print out the values in positions 3,4, and 5 of out columns means variable
myColumnMeans[3:5]
#We can then input this into the mean function to ge their mean and assign it to a new variable
baseMean <- mean(myColumnMeans[3:5])
#following the same pattern (but updating the index numbers for the bits of data we want) we can get the other means
controlMean <- mean(myColumnMeans[6:8])
expMean <- mean(myColumnMeans[9:11])


#TASK 2####
#Calculate the mean for baseline, control and experiment, separated by condition (1=happy, 2=scary). Copy and paste the code here, and the results.

#There are multiple ways to do this in R but the simplest is to use a function called by()
#Check the documentation and you can see that this function want 3 inputs
#First is the data (in our case Lab_12_data)
#Second is what we want to group the data by (in our case Lab_12_data$Condition)
#Third is the function we want to apply to the grouped data (in our case colMeans)

#So we can write
groupedMeans <- by(Lab_12_data, Lab_12_data$Condition, colMeans)
# If you look in the environment panel after running the line above and double click on the variable, you will see it looks a bit different from
#the dataframes or numeric variables we have seen so far.
#This type of variable is called a list
#In the first element of the list are the means for each column in group and in the second element are the means for those in group 2
#To access data in a list the easiest thing to do is to use double square brackets [[]], like this 
gp1Means <- groupedMeans[[1]] 
gp2Means <- groupedMeans[[2]] 
#These two lines of code get use two separate variables (ones for the means of group 1 and the other for the means of group 2)

#We can then repeat the same kind of thing we use in task 1 to get the average of each task (across the 3 trials)
gp1BaseMean <- mean(gp1Means[3:5])
gp1ControlMean <- mean(gp1Means[6:8])
gp1ExpMean <- mean(gp1Means[9:11])

gp2BaseMean <- mean(gp2Means[3:5])
gp2ControlMean <- mean(gp2Means[6:8])
gp2ExpMean <- mean(gp2Means[9:11])


#TASK 3####
#Plot a line graph showing the first set of means – copy and paste here.

#We want to make a plot that has the value of the mean on the y-axis (the vertical one)
#However we also need to tell the function we will use to plot data where to place those data points on the x-axis (the horizontal one)
#The simplest is to place them at 1, 2, and 3, so I will create a new variable with these numbers
xValues <- 1:3
#Since we have stored the means for each task as separate variables, before we plot them we need to put them all in one variable
#The way to stick single values into one variable (called concatenation) is to use c()
yValues <- c(baseMean,controlMean,expMean)

#We now have one variable with all our y values and one with our x values so we can now plot a graph
plot(xValues,yValues)
#If you run the line of code above you should get a plot appearing in the plots panel (bottom right of RStudio)
#However, it has only plotted points for our data and has not joined them together using a line
#We can use a function called lines() to add the lines on top
lines(xValues,yValues)
#However, we also need to add some information to the axis labels to make this plot ready for other people to understand
#The code below will make it ready, please try to play with some of the parameters yourself to see how it changes the plot
#We are going to use things called optional input arguments to change some of the details
#In R we specify these after the main arguments (xValues and yValues in this case), and we specify them using a pattern.
#We first say what option we want to change, then we put an = symbol, and then what we want to change it to, 
#for example to change the x axis label to be Task we would write:
#xlab = "Task"
#You can use multiple of these optional input arguments at the same time and you can find details in the help for each 
#function
#I have specified the xlabel, ylabel, title and line colour. The final xaxt means that the function won't draw any
#details on the x-axis such as tick marks or labels, this is because I want to control them later using the axis()
#function
plot(xValues,yValues, xlab = "Task", ylab = "Mean", main = "Means for Each Task", col = "red",
     xaxt="n")
lines(xValues,yValues, col = "red",lwd =3) #I've made the line red as well and also changed the thickness to 3
axis(1, at=c(1, 2, 3), labels = c("Base","Control","Exp")) #here is where I tell it to put tick marks and give them labels
#You can use c() like this to stick other things like letters together as well

#TASK 4####
# Plot a line graph with 2 lines (one for each condition on the same graph) – copy and paste here.



