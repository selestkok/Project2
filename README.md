# MIST 4610 Project 2: Team 1

### Team Members: 
1. Emily Jackson [@edj69332](https://github.com/edj69332)
3. Parker Jackson [@jcp39649](https://github.com/jcp39649)
4. Selest Kok [@selestkok](https://github.com/selestkok)
5. Paola Diaz [@paoladiaz1](https://github.com/paoladiaz1)
6. Lukas Farris [@Lafarris824](https://github.com/Lafarris824)

### The Dataset 
We picked this data set from the US Data gov website. “Animal Shelter Animals” originates from the Bloomington Animal Shelter, specifically during a system migration in early 2017 when they switched from using AnimalShelterNet to a new management software called Shelter Manager. This data is continuously updated, with the last update being from April 19, 2025. The dataset captures records of individual animals handled by the shelter, and final outcomes (such as adoption, death, or transfer). Our dataset contains 39,013 rows and 23 columns. A few examples of some of the dimensions are id, Intake date, Intake reason, Is transfer, Shelter code, Animal name, and Breed name. 

## Question #1
### Is it possible to determine the number of most common animals in the shelter during a specific month? 

### Q1 Visualization and Results
![Number of Animals by Month](https://github.com/user-attachments/assets/82df9cd3-e98e-42ac-aa9c-2e571ffa3e1b)
Predicted Data for dogs: <img width="409" alt="Count of Id = -0 519684Month of Intakedate^3 + 3 81341Month" src="https://github.com/user-attachments/assets/b2918363-d431-4913-80e9-6143db72511e" />

Predicted data for cats: <img width="411" alt="Count of Id = -4 00505Month of Intakedate^3 + 25 6132Month" src="https://github.com/user-attachments/assets/fe253397-71ac-42c4-874d-4e9af182271e" />

### Q1 Importance 
Cat intakes spike dramatically between April and August, matching typical “kitten season” trends, with a sharp decline from August to December. Dog intakes stay relatively stable year-round. Knowing which animals are most present in each month helps shelters plan for space allocation, staffing needs, and supplies. If certain animals tend to flood the shelter during certain months (kittens in spring), the shelters can run targeted adoption drives and partner with rescues for overflow. The huge seasonal spike in cats means the shelter needs extra space, food, foster homes, and staff during Spring/Summer. Since dog intake is steady, year-round dog care planning is easier. But there may be capacity competition during cat season. Overcrowding specific species without planning can lead to stress and illness, and understanding common influx patterns allow shelters to proactively maintain better welfare conditions.

### Q1 Manipulations
No manipulations were used in this question

## Question #2
### Is there a significant difference in the percentage of animals put to sleep among the different reasons for animal intake?

### Q2 Visualization and Results
![AGV_vUc3GbpVfqB4WKw4a2aSxJ0LlBWzqVegPdjSdHXhmGO6pCrQ8DipcITRiKk6b46fEd8BghL93dlkNw99uH9yLBWZRtCFbw1KiSLbNEfKdoG---exdWhCYLty](https://github.com/user-attachments/assets/550fbc9d-c4c3-48e0-b451-5e757c73e272)

### Q2 Importance 
This question is important because knowing what intake reasons lead to a high likelihood of being put to sleep allows the shelter to focus more on animals brought in for those reasons. If the intake reason has to do with returned pets due to poor behavior  for example, they can allocate more resources and attention to training those pets. The hope of this extra focus would be to decrease the percentage that are put to sleep, and increase the percentage that are released into the wild or adopted.

### Q2 Manipulations
We created Created new variable in excel sheet called PTS_True*1. This variable codes all animals that were put to sleep as 1 and others as 0. This variable allowed the creation of a new calculated field in Tableau called  “Percentage Put To Sleep”. This field shows the percent of animals for that intake reason that were put to sleep  divided by the total number for that intake reason.
![AGV_vUc2Jt5t50BritoDtgoEjupqHIuA0kmzKEI5SM2VCaJG2kZ4nIiWrPg9FUmVuoLpcUiOfv8y42n1-aRGInPJKJ4jAX5UvzeB7VlTWwhEVEMO3V2oa2WO_mcK](https://github.com/user-attachments/assets/3bf5e46b-6a2c-43e4-a8d6-0eaaafa3f958)

![puttosleep PTS_True1](https://github.com/user-attachments/assets/4be12ff3-f513-4b74-81f1-accc76199c31)


