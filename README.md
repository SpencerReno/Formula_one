# Formula One (WIP)
Data analytics on Formula One data from 1950-2021

## Constructors Decade Placings
For all current ten teams that are actively competing, this is their placing over the last decacde. If a team has changed Its name but stayed under the same parent company that has been accounted for and combined under their most recent team name.

![Decade placings](https://user-images.githubusercontent.com/88803320/148436822-8e22790c-13fa-47b1-928b-c9fc56c662af.png)


## Abu Dhabi Pit Times 2020 - 2021
This graph compares the pit times between the 2020 and 2021 Abu Dhabi Grand Prix. The Abu Dhabi Grand Prix is the final race for both of these seasons so stakes are always high. Not all drivers are included in this graph due to certain circumstances. This could be either they did not compete in both 2020 and 2021 seasons or the driver retired their car before completing one full pit. This graph shows a good comparison of how the teams did with their fastest pit stops from each race. Half of the drivers included did better in 2021 than 2020 while the other half fell short. 
![pit times 2020 2021](https://user-images.githubusercontent.com/88803320/149194071-d50e8ab1-c5b9-40ab-9618-7e41747c4d95.png)

## Abu Dhabi Position Change Graph
Position Changes perlap from the 2021 Abu Dhabi Grand Prix. Mazapin is not included as he did not fully complete a lap in the race. A lot of the positions changes happend from lap 14 to lap 24 as this was the main pit window for most teams on soft and medium tyres. 
![lap placement](https://user-images.githubusercontent.com/88803320/149990560-7b913525-e348-4149-9512-b8a456b03f03.png)


## Machine Learning 
The best way to keep the values even between each team is to track only the last 10 years. It would be unfair to track Farrari vs Haas when Farrari have been competing since the 1950s and Haas only joined in 2016. With That being said this is a machine learning model to predict the constructor placements based on previous years placements. 

This graph below compares the two scores from the random forest model and the kneighbors model. Both had great train scores up in the high 90s, but the testing scores differed with Kneighbors taking the advantage for a score just be low a 96.

![ModelScores](https://user-images.githubusercontent.com/88803320/151215124-b49b9b65-6fde-4438-90ad-4f7d92902368.png)