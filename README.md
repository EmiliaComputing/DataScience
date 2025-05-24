# Data Science
These are data science projects.

## Prices
(completed 2022)

### Introduction
I chose to create this project because I wanted to develop a greater understanding of data science. This project uses training data to learn how to predict the average cost of houses in an area. To predict the price, this project requires the user to input four integers, the total number of rooms, the total number of bedrooms, the median age of the housing and the number of houses in the area. 

### Project Goals/Requirements
I decided to code this project using python because I wanted to create a text based program which would enable the user to input data and I felt that this programming language would be most suited to me developing a project with these features. 

### Design
The user interacts with the computer by text. They are asked to input data into the computer. There are no buttons, typing into a box is the only way in which the user can interact with the program.

Firstly, the algorithm imports what is necessary to perform the needed operations and checks the data before displaying it in a series of tables. Then, certain features from the data (the total number of rooms, the total number of bedrooms, the median age of the housing and the number of houses in the area) are selected to estimate the average price of housing in that area. A new graph is shown which only displays these components. The user then inputs a value for each of these before the computer predicts what the average price of housing in that area would be. The number printed at the bottom is the average price of a house in that area.

The code below shows how the computer calculates the average house price. It is written in python.

    room_new = int(input("Enter number of rooms in the new area: "))

    bedroom_new = int(input("Enter the number of bedrooms in the new area: "))

    median_age_new = int(input("Enter the median age of housing in the new area in years: "))

    households_new = int(input("Enter the number of households in the new area: "))

    new_area={"total_rooms":[room_new],
              "total_bedrooms":[bedroom_new],
              "housing_median_age":[median_age_new],
              "households":[households_new]}

    new_area_df = pd.DataFrame.from_dict(new_area)

    predictions = housing_price_model.predict(new_area_df.head())

    print(predictions)
 
The first four lines are when the user inputs the data, the next four are a dictionary which is made containing the inputted data, the following two are how the computer calculates the average price and the final line prints the predictions.


### Evaluation
I feel that this project went well as it enabled me to successfully achieve a greater understanding of how computers learn and I was able to create a project which analysed data and was able to make predictions based on that data.

## Sentences
(completed 2022)

### Introduction
I decided to create this project because I wanted to gain a greater understanding of data science and how artificial intelligence is used to gather information. This project decides which words in a sentence are important and which are not.

### Project Goals/Requirements
I decided to use python to create this project because I wanted to create a text based program that could analyse data which would enable the user to input data and I felt that I would be able to best create this if I used the programming language python.

### Design
This program does not have a graphical user interface and this is a text based program, therefore the user interacts with the computer by inputting data using text. There are no buttons as the user uses the keyboard to type the data which they wish to input. 

Firstly, the program imports what is necessary to perform the needed operations and to analyse the sentences. The program then tells one of those installations, “spaCy” that the language which these sentences are written in is English. Next, the program prints out a statement saying that if the word “True” is printed next to the word, then it is unimportant. However, if the word “False” is printed next to the word, then it is important. The user then inputs a sentence and the computer determines whether each word contributes to the overall meaning of the sentence or not.

Afterwards, the computer uses the phrase matcher which was imported from spaCy to decide what an extract from a website is most likely to be talking about out of a given list of words.

### Evaluation
I feel that this project went well as it enabled me to successfully achieve a greater understanding of how computers learn as well as how they analyse text and data. Additionally, I was able to create a project which analysed text and was able to make statements based on that data.

## Global Warming Project
(completed 2022)

### Introduction
I chose to create this project because I wanted to develop a greater understanding of data science. This project attempts to prove that climate change is real by drawing graphs showing the average temperature rising whilst the uncertainty about those temperatures is going down. 

I think that programs like this are important as they show the extent of climate change and also prove that it is real.

### Project Goals/Requirements
I decided to code this in python because I wanted to use “matplotlib.pyplot” to draw the graphs and present the data. I also wanted to use “pandas” to allow the computer to read the data. Additionally, I felt that python would be the language where I could best create a project which would display data.

### Design
This program does not have a user interface, its only purpose is to display the data contained in the data sets. There is no way for the user to interact with the computer. 

Firstly, the computer imports what is necessary to read the files and present the data showing the average temperatures, which was downloaded from a website. The computer then draws a table of the data. Afterwards, the computer calculates the average temperature and the average deviation. Then the computer shows graphs proving that the average temperature is going up whilst the uncertainty is going down.

### Evaluation
I felt that this project went well because I succeeded in creating a project which could display data of the average temperature each year in the form of graphs in order to prove that climate change is happening as the user would be able to see a rise in the mean temperature. 

A project like this would improve how we look at climate change in the future because it shows how rapidly temperatures are increasing and it also shows that climate change is happening.

## Chess Analysis
(completed 2022)

### Introduction
I decided to create this project because I wanted to design a project which could analyse chess games and plot graphs based on the fifty most common openings, the different possible outcomes of games and the most common ratings. I chose to make this project about chess as it is a game which I enjoy playing.

### Project Goals/Requirements
I chose to code this using python because I wanted to use “matplotlib.pyplot” and “seaborn” to draw the graphs and present the data. Additionally, I also decided to use this programming language because I feel that python is the language where I can best create a project which would include data and analysis. 

The end purpose of this project is to present data about chess games in a series of graphs.

### Design

This project does not have a user interface, its only purpose is to display the data contained in the data sets. There is no way for the user to interact with the computer.

The program firstly imports “pandas”, which is used for reading the data, then it imports “matplotlib.pyplot” to draw the graphs and present the data, next it imports “seaborn” which is used for making statistical graphs. Afterwards, the computer loads the data and presents it in a series of tables. Then the computer plots the graphs: firstly the results, then the ratings and then how many times the fifty most common openings were played.

### Evaluation

I feel that this project went well because I successfully created a project which could analyse data and present it in a series of graphs which showed different statistics about chess games.


## Phone Reviews
(completed 2022)

### Introduction
I chose to create this project because I wanted to develop a greater understanding of data science and natural language processing. This project uses training data to learn how to determine what the star rating of a review would be based on the words in that review.

### Project Goals/Requirements
I chose to develop this program by using python because I wanted to use “spaCy” for the natural language processing and “pandas” for reading the data. I also wanted to use python because I decided to create a text-based program and I thought that python would be most suited if I were to create a project with this requirement.

The end purpose of this project is for me to develop a greater understanding of using computers to create data science projects, analysing data and natural language processing.

### Design
This is a text based program. The user interacts with the computer by typing a review into a box. The computer then decided whether this review is positive or negative and gives it a “star rating”. This rating goes from a series of one to five, with one being the worst and five being the best. The computer prints out a number followed by a decimal number. 

    {'1 star': 0.42582544684410095, '2 stars': 0.3665180206298828, '3 stars': 0.3938756585121155, '4 stars': 0.4008767902851105, '5 stars': 0.49512746930122375}

The higher the number, the higher the likelihood that the review being given that star rating.

### Issues during the project
There is an issue with this project. Despite the project being accurate when dealing with positive reviews, it is not accurate when the reviews are negative. When the reviews are negative, they are given higher, more positive star ratings than they should be. A possible cause of this is the data set which I use for this project.

### Evaluation
I think that this project went well because from this project I developed a greater understanding of using computers to create data science projects, analysing data and natural language processing. 

I also created a project which could determine the star rating of a review based on training data.

However, this project was not accurate when the reviews were negative. A possible cause of this is the data that I had used whilst making this project. Therefore, if I were to do this project again, I would use a different data set.
