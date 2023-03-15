<h1>Smart Watch Data Analysis</h1>



<h2>Description</h2>There is a lot of competition among the brands in the smartwatch industry. Smartwatches are preferred by people who like to take care of their fitness. Analyzing the data collected on your fitness is one of the use cases of Data Science in healthcare.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Python</b> 
- <b>Jupyter Notebook</b>


<h2>Program walk-through:</h2>

<p align="Left">
Launch Jupyter Notebook & Import Necessary Libraries<br/><br/>
<img width="940" alt="s1" src="https://user-images.githubusercontent.com/65899924/225303527-48f31dbd-7d8e-428f-8747-e343a3bfb1c8.png">


 <p align="Left">
 Before moving forward, let’s have a quick look at whether this dataset contains any null values or not: <br/><br/>
<img width="932" alt="s2" src="https://user-images.githubusercontent.com/65899924/225303744-245344fd-6ac5-4bb2-9959-bb8ada423308.png">



<p align="Left">
The dataset doesn’t have any null values:<br/> <br/>
<img width="946" alt="s3" src="https://user-images.githubusercontent.com/65899924/225304043-873d37be-5360-407d-be97-6dadda5c6200.png">
 




<p align="Left">
The column containing the date of the record is an object. We may need to use dates in our analysis, so let’s convert this column into a datetime column: <br/>
<img width="941" alt="s4" src="https://user-images.githubusercontent.com/65899924/225304675-bc4d46f9-34f9-45c1-bcf8-20deb5e809ff.png">
 



<p align="Left">
Look at all the columns; you will see information about very active, fairly active, lightly active, and sedentary minutes in the dataset. Let’s combine all these columns as total minutes before moving forward:

<img width="940" alt="s5" src="https://user-images.githubusercontent.com/65899924/225305209-cbc728db-1f89-4d69-88fa-8c50d803e562.png">
 






<p align="Left">
Now let’s have a look at the descriptive statistics of the dataset: <br/><br/>
<img width="939" alt="s6" src="https://user-images.githubusercontent.com/65899924/225306198-5b983bf5-59fc-4d2c-8e41-13ffd56bcdb7.png">
<img width="944" alt="s66" src="https://user-images.githubusercontent.com/65899924/225307235-560ac407-8932-41b9-a0d7-22062939175f.png">

 


<p align="Left">
<b>Let’s Analyze the Smartwatch Data⌚️</b><br/><br/>
The dataset has a “Calories” column; it contains the data about the number of calories burned in a day. Let’s have a look at the relationship between calories burned and the total steps walked in a day: <br/><br/>

<img width="943" alt="s7" src="https://user-images.githubusercontent.com/65899924/225307477-38cb5543-5d92-42eb-b67d-a2a73e06342b.png">
 
<p align="Left"> 
You can see that there is a linear relationship between the total number of steps and the number of calories burned in a day. Now let’s look at the average total number of active minutes in a day:
 

<img width="931" alt="s8" src="https://user-images.githubusercontent.com/65899924/225308148-3c5fc014-6f1e-4f41-952d-f8710bbf42f6.png">
 
![s88](https://user-images.githubusercontent.com/65899924/225308199-3e41ac43-9a21-48e4-bdef-8539f700ea21.png)
 
 
<h3><b>Observations:</b></h3>
1)81.3% of Total inactive minutes in a day<br/>
2)15.8% of Lightly active minutes in a day<br/>
3)On an average, only 21 minutes (1.74%) were very active and 1.11% (13 minutes) of fairly active minutes in a day<br/><br/>
 
  
<p align="Left">
 We transformed the data type of the ActivityDate column to the datetime column above. Let’s use it to find the weekdays of the records and add a new column to this dataset as “Day”:

<img width="939" alt="s9" src="https://user-images.githubusercontent.com/65899924/225309357-46f63c1b-e2d6-4301-b25f-7b4bf7d76724.png">

 
<p align="Left">
Now let’s have a look at the very active, fairly active, and lightly active minutes on each day of the week:<br/>

<img width="943" alt="s10" src="https://user-images.githubusercontent.com/65899924/225309640-c1288e01-078c-44f7-9799-857b8a4bca68.png">
 
![s1010](https://user-images.githubusercontent.com/65899924/225309706-33f1d228-a725-4735-b132-64ba81eae126.png)
 

<p align="Left"> 
Now let’s have a look at the number of inactive minutes on each day of the week:<br/><br/>

<img width="940" alt="s11" src="https://user-images.githubusercontent.com/65899924/225309972-07d3871e-99fa-4bd3-bef7-6aa482f5840c.png">
 
 
<p align="Left"> 
<b>So Thursday is the most inactive day according to the lifestyle of all the individuals in the dataset.<br/><br/></b>
Now let’s have a look at the number of calories burned on each day of the week:
<img width="938" alt="s12" src="https://user-images.githubusercontent.com/65899924/225310292-c64601bd-167d-4655-8d6e-380fe281547e.png">
 
![s1212](https://user-images.githubusercontent.com/65899924/225310372-7a0755cf-ed61-4a2a-8df8-b5b121bfef0e.png)
 
 
 
 
<br/> 
 
<h2><b>Summary:<br/></h2>
Tuesday is, therefore, one of the most active days for all individuals in the dataset, as the highest number of calories were burned on Tuesdays.<br/>

So this is how you can analyze smartwatch data using the Python programming language. There is a lot more you can do with this dataset. You can also use it for predicting the number of calories burned in a day. </b>
 





