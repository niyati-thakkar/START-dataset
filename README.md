


# ![ref1]
<a name="_omamt3oo8cik"></a><a name="_odl31ay5cq5a"></a>**DATA MINING AND ANALYSIS - START DATASET**

<a name="_ed8c8ns4fgez"></a>**CASE STUDY**

# ![ref2]
# <a name="_921gikj9xv3d"></a><a name="_91k9guql50j9"></a><a name="_940bn1q2chx1"></a><a name="_neox3iubf91n"></a>**TABLE OF CONTENTS**

1. Executive Summary ……………………………………………………………………………………......…….. 1

1. Background …………………………………………………………………………………………………….…….. 2

`		`2.1 Misconceptions about Terrorism ............................................................................. 2 

2\.2 Factors affecting Terrorism ....................................................................................... 3

2\.3 Dataset Challenges ....................................................................................................... 4 

2\.4 Datasets ............................................................................................................................. 5

1. Case Evaluation ……………………………………………………………………………………………………. 6

1. Proposed Solution …………………………………………………………………………………………..……. 7

4\.1 Project Design ................................................................................................................. 7 

4\.2 Data Preprocessing …………………............................................................................... 7 

1. Conclusions ………………………………………………………………………………………………...………… 9

1. Recommendations ………………………………………………………………………………………...……. 10

1. Implementation/ Demonstration ……………………………………………………………………...... 12

1. References ………………………………………………………………………………………………………….. 21
#


# ![ref2]
# <a name="_6m8agwozlxug"></a><a name="_jkdlhdn097pz"></a><a name="_7lbkqttrdqy0"></a>**Chapter 1:**
# <a name="_t4ebjjtroxpo"></a>**EXECUTIVE SUMMARY**

In this work, we present analytical results from data mining on the START (Study of Terrorism and Response to Terrorism) dataset. The main objective is to visualize terrorism data and make it available to users in an easy-to-understand format. 

Lack of understanding and awareness about global terrorism leads to diverse opinions and common misconceptions among civilians. In this age of globalization, sufficient information about this topic can help strengthen our counter-terrorism strategies, improvise security concerns, regulate better economic policies, and enhance the knowledge base of civilians.

The primary dataset for this project is provided by the START Consortium which contains data on terrorist events since 1970. Performing various data mining and data visualization techniques to interpret the nature of terrorism to better understand its trends and patterns in over 45 years of its recorded history.














# ![ref2]
# <a name="_sn1x97khan4i"></a><a name="_kcgtui27zbj2"></a>**Chapter 2:**
# <a name="_3nugau9bqzox"></a>**BACKGROUND**

**2.1 Misconception about Terrorism** 

Terrorism is sporadic, widespread, and inconsistent with time and nature. Because of these characteristics, International terrorism is difficult to summarise all aspects as a single conclusive solution and make this information available to be easily understood by most people. Exploring this dataset can provide insight into how different parameters are correlated with each other, which can help identify unknown hidden patterns. This exploration will also assert enough facts to provide justifications for some common misconceptions regarding terrorism. 
# <a name="_jujpvzp7ts1i"></a>**2.2 Factors Affecting Terrorism** 

Identifying dependent factors of terrorism is one of the goals of this project. There are parameters like religion or nationalism that are not defined in the dataset but have a major influence on contemporary terrorism. Religion has been a very controversial topic among researchers about whether religion influences terrorism or not and if it does, up to what extent is a bigger question. Conclusive evidence shows how religious idealization or belief can shape and transform terrorism. Religious idealization has been one of the major motivating factors leading to fanaticism and in turn, evolving into terrorism. Classification mining is done using a C4.5 algorithm with 10-fold cross-validation to generate a classification tree model resulting in an accuracy of 93.53% in predicting the correct set of events; Religious events being the major dependent variable.  Hence religion’s contribution to terrorism is an interesting subject to explore. 

**2.3 Dataset Challenges** 

START terrorism dataset has a marginally low occurrence of events occurring at the same geolocation. Most of the events are not consistent or do not occur frequently. Hence difficulty arises in making quantitative projections with varying degrees of similar events. As a result, different classification techniques provide different results. In this case, Lazy Classifier IBK, Linear NN search, and Filtered Neighbor Search techniques provide higher accuracy on the dataset compared to Naïve Bayes, Multiclass Classifier, and Multilayer perceptron. This helps in understanding which techniques and methodologies are more effective for similar analysis on this dataset. 

Another major challenge while working on this dataset is that individual studies lead to different conclusions. Current shortcomings and limitations in data collection techniques, definition debates, and irregularity in coding and analysis give rise to disagreements among researchers and in turn, rule out their conclusion. An acceptable level of theoretical and empirical analysis is required to prove a heuristic casual model showing links between globalization and terrorism. One of the issues is critical disagreement over the definitional debates around various terrorist events that exert a detrimental influence on this field’s development. This issue demands the exercise of a need for common grounds that can be accepted by most experts and concerning authorities to agree on what could be the standard norms and procedure to be considered as a legitimate piece of information on terrorism on which appropriate research can be done. A 5 Podcast by Gary Lafree is an excellent example that shows how terrorism even though being a collection of facts for researchers, often concludes with diverse results, sometimes contradictory to each other. Hence research and analysis done in this project are heavily based on the information provided by Global Terrorism Dataset and our study might vary from other research depending on the different sources used in the process.

**2.4 Datasets**

The primary dataset used in this project is called the START (Study Terrorism and Response to Terrorism) dataset which is a part of the Global Terrorism Database, compiled by the START consortium. START dataset is an unclassified, open-sourced, freely available dataset for anyone to use and has the most comprehensive collection of terrorist events among all other available datasets. START dataset contains data of more than 180000 terrorist events that have happened since 1970 and has over 120 variables describing each attack. Some of the key attributes consisting of those variables which are used for this project are listed below in Figure 1:


|**Attributes**|**Description**|
| :-: | :-: |
|Attacktype1\_txt|<p>The type of attack that happened. Attacktype1\_txt consists of categories like an explosion, armed assault, assassination, kidnapping, and unarmed assaults.</p><p></p><p></p><p></p>|
|Target1\_txt|Type of target involved in the attack. Target1\_txt consists of categorical values like private citizens, military, police, government officials, transportation, education, religious institutions, airports, etc.|
|Success|‘1’ if the attack was a success. ‘0’ if the attack was a failure.|
|Multiple|Value for the number of attacks conducted in a single terrorist event.|
|Natlty1|Nationality of the attacker.|
|Weaptype1|Type of weapon used in the attack. Weaptype1 contains values like firearms, explosives, melee, vehicles, etc.  |
|Nkill|Number of people killed in any event|
|Nwonded|Number of people wounded in any event|
| |Organisation that claimed responsibility for an attack|
|Region\_txt|Name of the region where the attack happened. Region\_txt consists of values like East Asia, South Asia, Western Europe, etc|
|Longitude|Longitude of the location|
|Latitude|Latitude of the location|
|Property|Total property damage happened in any event|
|Suicide|‘1’ if the attack was a suicide attempt. ‘0’ if the attack was not a suicide attempt.|
|Motive|Known motive of the attacker|
|Age|Estimated age of the attacker|
|Day, month, year|Calendar details of the event.|
# <a name="_yjnex5wgxdot"></a>***Figure 1. Description of dataset key attributes*** 
Other similar terrorism-based datasets used for references are

`        	`**ITERATE:** ITERATE stands for International Terrorism: Attributes of Terrorist Events. This dataset is copyrighted and is not available as an open-source resource for external users. ITERATE mostly includes transnational incidents involving terrorist groups, their activities, and their environment of operations.

**RDWTI:** RAND Database of Worldwide Terrorism Incidents includes incidents from 1968 until 200.  However, RDWTI includes both types of events; transnational and domestic. More than 40,000 incidents are recorded and detailed in this database offering comprehensiveness and quality to the users.

**INSCR:** Integrated Networks for Societal Conflict Research is a collection of multiple individual datasets like High Casualty Terrorist Bombing (1989-2019), Coups d’état (1946-2018), State Fragility Index and Matrix (1995-2018), India SubNational Problem Set (1960-2004) and many more. These datasets are quite focused and cover diverse topics about the impacts of terrorism on other sectors like civil wars, local crime rates, political changes, immigration, etc. 







# ![ref2]
# <a name="_pz6ce3ic1vyt"></a><a name="_1pvo6y76ru8q"></a>**Chapter 3:**
# <a name="_e0u8nlwvtsto"></a>**CASE EVALUATION**

The problem statement here is to build a tool that can present processed information in the form of an intuitive visual representation of analyzed data. Implementation of this project involves system design, backend design, visual design, and user interface. 

System design includes the overall design plan of the whole project system which explains how each module is correlated with others.

The backend design contains a series of data preprocessing steps to transform the raw dataset into a more meaningful and focused collection required for this project. This design module also includes scripts for analyses and other factual information derived from the dataset. 

Visual design mostly consists of analyses and visualization techniques to construct different graphics representing the results in an easy-to-interpret format. 

The User Interface is in the form of a user-oriented website to present and explain different visual analyses to provide a better understanding of the dataset. The user can interact with the dataset using the exploration tool.


# ![ref2]
# <a name="_ghpwzipoiiov"></a><a name="_x2cofmhwvo9p"></a>**Chapter 4:**
# <a name="_dhtpx9b1jqxz"></a>**PROPOSED SOLUTION**

**4.1 Project Design – Solution Approach**

Most of the operations on the dataset are done by python scripts on Jupyter Notebook which is an open-source web-based application for python code development. Python is used for data preprocessing, data modeling, analyses, and visualization. Anaconda is used as an open-source python distribution for handling Jupyter-based dependencies and provides a python environment for code development. These scripts are then executed by a python-based web framework – Django. A website is developed in HTML/CSS and JavaScript which is deployed on a Django server to communicate with Jupyter-based python scripts. Visualizations from those scripts are displayed on the website along with detailed explanations to help users understand and interpret the context. 

**4.2 Data preprocessing** 

Data preprocessing is the first step to be done after collecting data. It is a set of operations performed on the START (Study of Terrorism and Response to Terrorism) dataset to modify ambiguous data which can be a bottleneck to analytical results. Raw data is simply a collection of related information put together. Raw data is often unorganized and contains a lot of information that is irrelevant to the project requirements. Data preprocessing methodology helps in converting this raw data into a more meaningful, focused, interpretable, and readable format. 

The available START dataset from the Global Terrorism Database is incomplete and inconsistent and contains many errors, missing attribute values, contains outliers, incorrect tags, and duplicate entries. Data preprocessing can help resolve these discrepancies.

The following are the steps used in this project as a part of the data preprocessing methodology: 

**Data cleaning** is a process of filling in missing values, removing outliers, and handling inconsistencies in data. In the terrorism dataset, there are numerous fields like 'motives' or 'responsible organizations' that are missing either due to information not being available or that field was not relevant for that specific event. Fields like 'summary', 'claim\_mode', 'claimmode\_txt', 'guncertain', 'nperps' etc. are removed since they are not relevant to the analysis of this project. Fields like 'weapsubtype2', and 'weaptype3\_txt' have more missing values than valid entries. Hence such fields are also removed to reduce complexity. 

**Data integration:** In this step, conflicts among data are resolved. Different representations of the same data such as multiple subcategories of weapon type (weapsubtype1, weapsubtype2, weapsubtype3) are put together to avoid confusion and duplications. Fields with one-to-one correspondence like ‘country\_code’ and ‘country\_txt’ are mapped to avoid any conflicts. 

**Data transformation:** Here data aggregation, generalization, and normalization are performed. The dataset has multiple target/victim subtypes. All those subtypes were aggregated to represent one value by summation of all similar subtypes. This technique reduces the total number of attributes in the dataset and hence reduces the variability in the data. There are multiple categorical attributes present in this dataset belonging to the same superset. For example, the weapon Sub-Type has 4 different attributes which can contain one of the 27 different values. Those 4 attributes were generalized into one weapon SubType and 27 different categorical values were generalized into 12 domains. Values like a grenade, landmine, dynamite, etc. were classified under the ‘explosives’ tag. 

**Dimensionality reduction: The** START dataset has high data sparsity which increases its overall dimensionality. This method reduces the effectiveness of density-related operations like clustering and outlier detection. Multiple fields are having more missing or null values than valid ones. Some of them are ‘Mode\_for\_claim\_of\_responsibility’, ‘divert’, ‘kidhijcountry’ etc. which are of less significance to our project. Such attributes are removed to reduce dataset processing time, avoid the curse of dimensionality, and ease data visualization. However, some missing values in attributes like property\_damage and motives which are of high importance cannot be removed. In such cases, missing values were replaced by the mean value of corresponding attributes associated with the ‘responsible group’ attribute.



























# ![ref2]
# <a name="_ktho6in0n7w8"></a><a name="_9y0su4duhc5b"></a>**Chapter 5:**
# <a name="_vtsmn6hex5bl"></a>**CONCLUSIONS**

The goal of this project is to build a tool that helps users to understand and interpret the nature of terrorism. Users can perceive the START dataset through visual designs. A visualization that can be used to calculate the total number of attacks, total kill counts and location based on the selected region and year provides an interactive interface to explore this dataset. Users can understand various patterns, trends, and correlations in terrorism through visual interpretation and its provided explanation. Users can also explore the START dataset and other terrorism-related sources for additional research purposes provided by this tool. This work can be used by curious civilians, security-related policy-makers, international organizations hosting worldwide events, foreign investors, and academic researchers to understand terrorism and its nature.


# <a name="_i3izwqlh39bi"></a>**


# ![ref2]
# <a name="_udwlz0gcyj20"></a><a name="_x8m7f27dd9b6"></a>**Chapter 6:**
# <a name="_cppxj8wwonpc"></a>**RECOMMENDATIONS**

**Technologies Used** 

**Python:** Python is a high-level interpreted language that supports different platforms like Windows, Linux, Mac, Rasberry Pi, etc. Python can be used for creating web applications, and database systems, handling big data, and performing complex mathematical calculations. Python can be treated in an object-oriented, functional, or procedural way. Jupyter Notebook is a powerful tool to script python for data analysis and can contain live code, descriptive texts, and visualization which can be created and shared just like a document. 

**Jupyter Notebook** is highly used in statistical computation, data transformation, and various machine learning techniques. 

**Anaconda** is an open-source distribution for programming languages like Python and R to perform scientific computation. Anaconda handles the underlying dependencies, package management, and deployment for both of these languages and also provides the necessary support for data collection, manages multiple environments, and shares and collaborates on projects along with production-based deployment. For this project anaconda provided the environment needed to run Python and Jupyter Notebook. Anaconda was also responsible for managing required packages, libraries, and modules. Anaconda made this project workspace easy to operate by taking care of compatibility among various packages.

**Django:** Django is a Python-based framework used to develop web applications. Django is known to have one of the best open-source framework documentation to develop real-world applications. Django applications can be easily deployed and managed in a cloud environment. Here, Django provided a development environment for the design and implementation of the website. Django is responsible for executing the Python scripts on the backend, collecting all the visualization generated from scripts, and porting them to the website. 

**HTML/CSS:** is used to create static web pages. HTML along with CSS and JavaScript is most commonly used for designing the look and feel of a website. By far, HTML is more compatible with browsers than any other web-based scripting language. In this project, HTML was used to create a website that can incorporate all the analytical results and visualizations to be displayed with necessary explanations. 

**Python packages:** Following are some of the python packages used in this project.

**Matplotlib:** It is a 2D-based plotting package that provides required modules and functions. A developer can customize font properties, styles, axes properties, etc. 

**Pandas:** It is used for data analysis and manipulation. Pandas can convert data structures and dataset formats to data frames on which operations like loading data, renaming attributes, mapping, crosstab, sub-data frames, plotting, etc. can be performed. 

**NumPy:** It provides structures for multiple dimensional array objects and tools for related operations. NumPy is usually used for high-performance scientific computational tasks. 

# <a name="_pwcnx5dn1doa"></a>**


# ![ref2]
# <a name="_ksljusgbecn3"></a><a name="_bur7bkn9x863"></a>**Chapter 7:**
# <a name="_jowl09jbbem"></a>**IMPLEMENTATION/ DEMONSTRATION**

This chapter discusses the code and implementation phase of the project. All scripts are written in Jupyter Notebook. The primary source of data is the START dataset. All operations are performed on the START dataset to generate visualizations.

**Reading the Data:**

![](Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.003.png)

*Figure 1: Data preprocessing-rename*

Most of the column names of the dataset needed to be renamed for easy use and understanding as shown in Figure 1. A new column is created with the name casualties containing the sum of the values of the total number of people killed and wounded. Terror.head(3) will display the top 3 entries in the dataset along with their corresponding column name as we can see in the output below.

**Data Preprocessing:**

![](Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.004.png)

*Figure 2: Data preprocessing- isnull() output*

In Figure 2, Isnull() function will check if the entry is null, and sum() will perform arithmetic addition to return the schema to the dataset representing the total null fields in individual columns.

![](Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.005.png)

*Figure 3: Data preprocessing-dataset facts*

Factual information can be obtained by simply aggregating the values of certain fields as shown in Figure 3. For example, here values\_counts() will return the object with the decreasing order so the most frequently occurring element will be at the top. Accessing index[0] will return the first element which in our case is the name of the country with the highest number of attacks. Similarly in Figure 3, max() will return the largest value in the terror[killed] column, and idxmax() returns the index containing the maximum value in that column.

**Terrorist Activities Each Year:**

![](Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.006.png)

*Figure 4: Terrorist Activities Each Year* 

Summarizing all the terrorist attacks over the years can provide us an idea of how terrorism has evolved and at what rate has it impacted the world each year. Figure 4 shows data from 1970 to 2016 for the total number of attacks that happen each year. Terrorist attacks were quite low in numbers in the decade of 1970. Terrorism then had a fair rise in the 1980s and early 1990s and was considerably low in the next decade but then terrorism rose from early the 2000s topping the charts like never before in history. Hostile environment and global tension have increased because of the number of attacks in recent years. This observation can help investigate factors that adversely impacted the sudden rise in the number of attacks.

**Attacking Methods by Terrorists:**

![](Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.007.png)

*Figure 5: Attacking Methods by Terrorist* 

Different types of weapons and methods have been used by attackers. There are 8 categorical values for the defined attack type. They are unarmed assault, Infrastructure attack, kidnapping, barricade incident, hijacking, bombing/Explosion, armed assault, and assassination. These attributes can explain which are the most often used means of attack. 14 Figure 5 does reveal the potential target or focus of the attacker. For instance, unarmed assault attacks are usually focusing on specific individuals or a group of small people. Explosives and bombings are targeted toward a larger audience. Hijacking aims to achieve some sort of ransom in return. Here the graph pictures the total number of kill counts with respect to specific attacking methods used. Figure 5 uses the nine most used means of attacking based on the casualties caused. Explosions are the most common followed by armed assaults, assassinations, hostages, and so on. Here the total number of casualties by explosive weapons is almost double that of the next most attack which is armed assault. This observation indicates that most of the attacks were intended for civilians to spread terror among widespread targets.

**Favourite Targets:**

![](Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.008.png)

*Figure 6: Favourite Targets* 

The attacker always tries to make an impact by targeting their victims. Analyzing the type of target will help understand their objective and most likely their motives. Terrorism is driven by an ideology that tries to make a change or impose an ideology. Looking into the most commonly targeted attributes will signify the attacker’s objectives and terrorism in general. There are more than 100 distinct target types. These target types are generalized into 22 categories. Here Figure 4 shows that citizens, the military, the government, and the police are the most common targets. This graph explains that terrorist groups or individuals have a dislike towards the authority of the state or the nation. Their main focus is either to make a change at the political level or force their ideology on government forces by retaliating against their authority.

**Number of Terrorist Activities by Region:**

![](Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.009.png)*Figure 7: Number of Terrorist Activities by Region*

Figure 7 shows that Middle East and North Africa are the most terrorism-prone regions followed by South Asia. The Australian Region has experienced very few terrorist events. Collectively we can say that The African and Asian Continent experience the highest number of terrorist attacks.

**Terrorism Transition in Regions:**

![](Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.010.png)

*Figure 8: Terrorism Transition in Regions* 

Figure 8 provides more details about how terrorism has aged in various regions. Observing this pattern, we can see that there has been a noticeable rise and falls in the graph for all regions. 

**Top Affected Countries:**

![](Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.011.png)

*Figure 9: Top Affected Countries* 

Figure 9 shows some of the most affected countries are Iraq, Pakistan, Afghanistan, and India based on the total number of attacks. Peru is also one of the most affected countries according to Figure 9 but from previous results of Figure 8, we observed that Peru does not represent its current terrorism situation based on the total number of attacks. But the Figure 9 graph does explain how some countries are prone to violent actions and differences in ideology which can lead to extreme terrorism.

**Killings in Global Terrorism:**

![](Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.012.png)

*Figure 10: Killings in Global Terrorism*

Figure 10 shown above is another form of representing the total number of attacks based on years. The interesting part to notice here is to compare different years based on the total number of attacks. Each block represents a year. Larger the block, the larger the number of attacks faced in that year. Surprisingly six major blocks belong to the current decade (the 2010s). This observation emphasizes that some of the most violent years in the history of terrorism happened in this decade, especially in an era when terrorism has been given priority more than ever before. Different shades are used to make neighboring blocks more distinctive from each other.

**Attacks vs Killed**

![](Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.013.png)

*Figure 11: Attacks to Kill Comparison* 

Figure 11  lists the most countries affected by terrorism based on the total number of attacks. Another bar along with each country’s attack count is the number of total victims killed in those attacks combined for that country. Figure 11 can analyze kills to attack ratio for the most affected countries. For Iraq, that ratio is very high. The average kill for each attack is over 3. There are countries like the Philippines, Peru and the United Kingdom which 21 has faced an almost similar number of attacks but have a different number of kills. The United Kingdom has suffered significantly fewer casualties compared to the other 2 countries. This association can help differentiate the counter-terrorism strategies in different countries resulting in a different number of kills for the same number of attacks. This comparison among countries can be taken into considerations while devising new tactics against terrorism.























# ![ref2]
# <a name="_at4830l2sgnl"></a><a name="_ridmhiho5pg9"></a>**Chapter 8:**
# <a name="_27yf2ij9l6zs"></a>**REFERENCES**

[1] United Nations, “Chapter-1 Purposes and Principles,” [Online]. 

https://www.un.org/en/sections/un-charter/chapter-i/index.html 

[2] A. Z. Borda, “Why we react differently to terror attacks depending on where they happen,” [Online]. 

http://theconversation.com/why-we-reactdifferently-to-terror-attacks-depending-on-where-they-happen-57389 

[3] START organization, “Global Terrorism Database,” [Online].  https://www.start.umd.edu/gtd/about/ 

[4] Kaggle, “Global Terrorism Database,” [Online]. 

https://www.kaggle. com/ash316 

` `[5] START Consortium Organization, “Global Terrorism Index,” [Online]. 

http://visionofhumanity.org/app/uploads/2017/02/Global-Terrorism-Index-2016. pdf 

23

[ref1]: Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.001.png
[ref2]: Aspose.Words.2dc75703-4c40-4e51-ae95-9bcd8b3a8cce.002.png
