# Big Data Analytics for Healthcare
## Supporting health care in everyday life with the help of IoT and smart watches
1. Scenario description 

Back in the days the interaction between the doctor and the patient were limited to text/telecommunication and to doctor visits. Due to the Internet of Things (IoT), it is possible to monitor the health of patients continuously and to make recommendations based on it. 

IoT made it possible in the healthcare sector to apply remote monitoring. Massive amounts of health-related data such as daily activity, pulse, sleep patterns, and so on, from all wearables devices ( fitness trackers, smartwatches, smart clothes, biosensors, blood pressure monitors, glucose trackers, and any other electronic devices that people can wear on their bodies) are typically collected in real-time and digitally via the user’s smartphone. Then data is commonly transferred to a remote/cloud server where it can be retrieved by medical personnel. Data is characterized by at least the 3 typical V’s: volume (massive), velocity (speed), and veracity (various types and formats). The massive amounts of data get generated, stored and analyzed. The data stored from the wearables require proper management and analyses to be able to derive meaningful conclusions. If not, analyzing this data will be too complicated. Shortly, it is important to manage this data efficiently to be able to revolutionize it to valuable insights from which actions can be taken.

An example are the smartwatches which have the potential to support health care in everyday life by supporting self-monitoring of health conditions and personal activities. Various analytic tasks/techniques can be applied to analyze and predict the prevalence of cardiovascular disease using health-related data that can be easily measured by smart watch users.

<b> 2. Analytical tasks <b>

Extracting meaning from raw data (structured, unstructured, real-time, historical, etc)  for trends and actionable insights is called Data Analytics. This can be applied on different levels, for example: analyzing the existing data to make ad-hoc reports or by using the historical data to make predictions about the future. Healthcare has different data analytics types, some of them being: descriptive analytics, prescriptive analytics diagnostic analytics and predictive analytics. 

Within the project the focus will be on analyzing three analytical tasks to show a doctor how ten of his patients have been doing for the month February 2022. As it is a pilot version, there is some user input data asked but there is also already some automatic data generation based on the steps taken. In the future the doctor would also like to see some automatically generated data based on heart rate and blood pressure. 

Based on the self-monitoring of health conditions and personal activities scenario described above, three Analytical tasks will be carried out using the data measured and inputted by the user by the smartwatch. The analytical task are provided in the table below: 

![image](https://user-images.githubusercontent.com/117458345/218728020-b47fa72e-e147-49fb-ae99-64e210f5cf34.png)

<b> 3. Data description <b>

The data set will contain the following columns:

![image](https://user-images.githubusercontent.com/117458345/218728370-666f1fea-8c6e-4b15-8645-53e8f14bebac.png)

<b> 4. Spark implementation <b>

As for the spark implementation, it is attached as a Python notebook separately with this paper.

<b> 5. Results <b>

a. Categorization of the heart-disease patients (light active, fairly active and super active) based on the average amount of steps taken per day:

20% of the super active users were detected with heart diseases. 36% of the patients fall into the fairly active user category . The top patients are light users which form 44% of the group.

![image](https://user-images.githubusercontent.com/117458345/218728914-ec7e7d56-c490-43f8-a6ec-047c66e0da73.png)

b.  Comparison between the number of patients on daily basis under stress that are non-smoker/non-drinker and the patients who are smoker/drinker:

The number of patients under stress who are non-smokers and non-drinkers is 14. The number of patients who are smokers and drinkers is 61. There is a huge gap between these two groups, which suggests that there is a relationship between smoking, drinking, stress and heart diseases.

c. Computation of the average stress score of the patients with heart diseases:

![image](https://user-images.githubusercontent.com/117458345/218729540-da21a88f-2336-4a8b-a134-a10f8a06ac9a.png)


