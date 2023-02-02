# ACM Research coding challenge (Spring 2023)

![image](https://github.com/sahisagiraju/coding-challenge-2023-spring/blob/main/Screenshot%202023-02-01%20at%2010.06.57%20PM.png?raw=true)
I was initially curious to see how many of each stars were available. Nevertheless, we must go back to the task.

After given this data, my immediate question was to see how these stars would correlate with the HR diagram. After plotting the stars on a graph of Luminosity (L/Lo) vs Temperature (K), I noticed that they do not appear to be similar at all. In fact the data seemed erratic, without any clear trends.

![image](https://github.com/sahisagiraju/coding-challenge-2023-spring/blob/main/Screenshot%202023-02-01%20at%2010.07.04%20PM.png?raw=true)

Afterwards, however, after realizing that the HR diagram was given with a reversed horizontal axis and that both axis were in log form, I reset the chart and noticed the clear similarity. 


![image](https://github.com/sahisagiraju/coding-challenge-2023-spring/blob/main/Screenshot%202023-02-01%20at%2010.07.10%20PM.png?raw=true)

My chart definitely matched the HR diagram. This was cool but after comparing the diagram with my chart, I noticed that there were no “giants” as it was indicated on the HR diagram. Other than that, everything else seemed fairly similar- the downward trend representing the main sequence matched that of the diagram, and so did the super giants area on the top portion of the chart, and the white dwarves on the bottom, left half of the diagram. They were indeed consistent with the trends evident in the diagram.

My next observation was with certain matching axes that I noticed when I searched up HR diagrams. Many diagrams had axes parallel to each other with completely different variables. For example, in this HR diagram, the absolute magnitude was parallel to the luminosity, and the temperature was parallel to the spectral class. I wanted to see if luminosity was related to a star’s absolute magnitude.


![image](https://github.com/sahisagiraju/coding-challenge-2023-spring/blob/main/Screenshot%202023-02-01%20at%2010.07.16%20PM.png?raw=true)
(https://astronomy.swin.edu.au/cosmos/h/hertzsprung-russell+diagram)

![image](https://github.com/sahisagiraju/coding-challenge-2023-spring/blob/main/Screenshot%202023-02-01%20at%2010.07.22%20PM.png?raw=true)


Once again there appears to be no real correlation. So I once again decided to conduct the logarithmic version of these axes.

![image](https://github.com/sahisagiraju/coding-challenge-2023-spring/blob/main/Screenshot%202023-02-01%20at%2010.07.28%20PM.png?raw=true)


Now the data seems less scattered. There appears to be a negative slope, curving downwards. I conducted regression tests with different equations (linear, quadratic, etc.) and the power series had the greatest R2 value for the data. Therefore, this might be the most accurate formula used to represent the line of best fit for this data. The equation y = 1.19x-2.58 became the most accurate representation, with a R2 value of 0.723. Though this does not prove that luminosity is directly proportional to the absolute magnitude, it did tell us that there is roughly strong correlation between the two variables.

![image](https://github.com/sahisagiraju/coding-challenge-2023-spring/blob/main/Screenshot%202023-02-01%20at%2010.07.33%20PM.png?raw=true)


Although I plan to do more with the data, this is what I have prepared for now. In the future, my next steps would be to take the data apart. I would then separate the data into the four main categories (three in this case, as there appears to be no indicator of a giant in this group): giants, supergiants, main sequence, and white dwarfs. I would then like to create lines of regression for each of these groups and calculate how much each star varies from the equations. This would help to prove the HR diagrams more.

Moreover, I would plan to study a star's age and place on the HR diagram. I would plot a star on the HR diagram, then, based on how far along the main sequence it is (i.e. half way, almost at the end, beginning, etc.) determine its age. I would do this for stars along the main sequence and also for the other groups, and then compile all the data. With this new data regarding ages, I would compare the age with its real age (calculated by using its rotation rate) to see what the relationship is between a star's age and how far along it is on the HR diagram.
