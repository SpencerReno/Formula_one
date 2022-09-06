# Formula One (WIP)
Data analytics and machine learning on Formula One data from 1950-2021. Most of the visuals and machine learning models will be with recent years. 

# 2022 Season Analytics

## Driver Standings
Current driver point standing for the 2022 season (Belgian Grand Prix)
![driverstandings](https://i.gyazo.com/d4d33980a8a04a9db71f98690e5c686d.png)

Heres a Zoomed in graph on the battle for the lower half the the drivers who have less than 45 points as of the Belgian Grand Prix.

![zoomedingraph](https://i.gyazo.com/5cc9342a74f70c1bdf336f0a8c58deed.png)


## Team Standings
Current team standings for the 2022 season (Belgian Grand Prix)
![teamstandings](https://i.gyazo.com/2a2d72403a7bd48da6b1743137d9977d.png)


# General Analysis 
## Constructors Decade Placings
For all current ten teams that are actively competing, this is their placing over the last decacde. If a team has changed Its name but stayed under the same parent company that has been accounted for and combined under their most recent team name.

![Decade placings](https://user-images.githubusercontent.com/88803320/148436822-8e22790c-13fa-47b1-928b-c9fc56c662af.png)


## Abu Dhabi Pit Times 2020 - 2021
This graph compares the pit times between the 2020 and 2021 Abu Dhabi Grand Prix. The Abu Dhabi Grand Prix is the final race for both of these seasons so stakes are always high. Not all drivers are included in this graph due to certain circumstances. This could be either they did not compete in both 2020 and 2021 seasons or the driver retired their car before completing one full pit. This graph shows a good comparison of how the teams did with their fastest pit stops from each race. Half of the drivers included did better in 2021 than 2020 while the other half fell short. 
![pit times 2020 2021](https://user-images.githubusercontent.com/88803320/149194071-d50e8ab1-c5b9-40ab-9618-7e41747c4d95.png)

## Abu Dhabi Position Change Graph
Position Changes perlap from the 2021 Abu Dhabi Grand Prix. Mazapin is not included as he did not fully complete a lap in the race. A lot of the positions changes happend from lap 14 to lap 24 as this was the main pit window for most teams on soft and medium tyres. 
![lap placement](https://user-images.githubusercontent.com/88803320/149990560-7b913525-e348-4149-9512-b8a456b03f03.png)

## 2022 Car Vs 2021 Car At Bahrain Quali
These three graphs show the time differance from the 3 qualification rounds at Bahrain in both 2021 and 2022. Clearly the 2022 car is slower than the 2021 car this was to be expected with some restrictions that were put in place by the FIA. The closest time comparison that could be made is with the Ferrari in q2. This is the closest any 2022 car has been to the 2021 times in the Bahrain race. In 2021 the Ferrari set a time of 1:30.010 and in 2022 the car set a time of 1:30.932. Almost one second slower which in the formula one world is a win vs a loss. This is however the first race of the 2022 season and the teams are just now dialing in the cars. Over time in the 2022 season the cars will become more competitive to the 2021 times as the teams find ways to get more time out of the car.
![Qual One](https://i.gyazo.com/fff7eebba75b39f0bf424b8a8cc052fe.png)

![Qual Two](https://i.gyazo.com/32836c92bc8b344edb03f7845b482f89.png)

![Qual Three](https://i.gyazo.com/e321617efa60f5e51fb774c103cbddd7.png)


## Machine Learning 
The best way to keep the values even between each team is to track only the last 10 years. It would be unfair to track Farrari vs Haas when Farrari have been competing since the 1950s and Haas only joined in 2016. With That being said this is a machine learning model to predict the constructor placements based on previous years placements. 

This graph below compares the two scores from the random forest model and the kneighbors model. Both had great train scores up in the high 90s, but the testing scores differed with Kneighbors taking the advantage for a score just below a 96. Aswell, the Kneighbors model determinds its values by the most nearest values. And when predicting team placings you want to find the ones that are nearest to eachother as they will be similar in value. For example a 1st place will be near another 1st place, 2nd will be near other 2nds and so on.

![ModelScores](https://user-images.githubusercontent.com/88803320/151215124-b49b9b65-6fde-4438-90ad-4f7d92902368.png)