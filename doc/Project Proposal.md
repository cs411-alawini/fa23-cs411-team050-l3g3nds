## Team-050 l3g3nds Project Proposal

### Project Title: Game Finder

### Project Summary:
Our project will allow users to find new games to play with ease. It comes with features to search for a game just based on a few key words. We plan on implementing this using a similarity function (possibly LIKE in SQL) to extract keywords so that the user can find a matching game. Users can also find a game through some preset filters. The ones we plan on using are Genre, Price, Platform, and Rating. We’re planning to preset searches to this filter (if the user doesn’t want to use the search by words by feature) as these filters are pretty general and will produce good results.
After the user performs the search, the results will appear below. These results can then be sorted by the user using a drop down feature. Sorting will allow the user to refine through more filters like number of players, language, application size, and more. We are planning on trying to implement a way to create a new database which corresponds to new games found and the keywords searched to find this game. This will be based on user feedback so that maybe in the future the searching for a game based on keywords will be done using this new database.

### Description:
Gaming has become increasingly complex in recent years. Users constantly need to know what computer requirements are needed to play certain games, external hardware support, etc. Our product will allow people to easily access this information, as well as other important attributes such as price and genre, to figure out if the game is the right fit for them.
Additionally, gaming has become increasingly popular, and with hundreds of thousands of games on the market, our product aims to filter a catalog for a user based on what the user is looking for in a game. For example, a user can input that they are looking for a horror game and our product will display the catalog of games that match what they filtered for.  
- **Data stored in the database: All of the attributes/fields currently stored in the database are described here: https://data.world/craigkelly/steam-game-data/workspace/project-summary?agentid=craigkelly&datasetid=steam-game-data. 
To briefly summarize, there are 78 fields stored that essentially describe different attributes of various STEAM games. These data fields include descriptions of the genre, the description of the game, hardware requirements, categories, price, age requirements, and much more. The data was compiled by a user named CraigKelly, and the GitHub for their project can be found here. 
- **Basic functions of our web application: First, users can create a profile with the basic login information and then are allowed to modify their profile later on as well. Users can search for the titles of video games using the filtering and search features. When a user searches for a title, our app will query the database and retrieve certain attributes of the related video game. The dataset provides a plethora of information (78 columns) and the user should be able to specify if they want further information such as the description/about section for a video game. 
- **Creative component that improves the functionality of our application: The creative component of this project would be that a user of this application would be able to find new games to play based on genre, description, price, and platform inputs. This would allow the user to seamlessly explore new games without having to search the internet for new games. Also, this feature would not return just 1 game that’s ‘matched’ to the user’s specifications, but multiple games that are ranked by # of downloads, price, or other factors they wish to interactively sort it by. 
	To achieve this we plan on using a good number of the 79 columns listed to allow the application to be user-friendly and interactive. By using different columns to act as different filters, and by allowing the returned results to be ranked by some sort of similarity matching we can achieve the level of user interactivity that we desire.

### Usefulness:
Plenty of applications and websites such as Steam and Epic Games have libraries that compiles all their games and related information. Our application will share a lot of the useful features with these libraries. However, our application will be dedicated to this feature and will make searching up games and their attributes incredibly easy for users.
Websites such as steam and epic games can’t sort by more niche attributes such as “computer hardware requirements” so if a user wants to determine if they are able to even play the game they would have to search the game up and scroll to find the hardware requirements. Our platform will make this easier and allow users to sort by this category as well as others. 

### Realness:
Our data is a compilation of game titles and the related game attributes. The data contains information such as a game's computer requirements, age requirements, price, etc. We can retrieve this data from the “Steam Game Data” link in the provided TA dataset doc. 

### low-fidelity UI mockup:


### Functionality: 

Our web application, based on the YouTube Video Trending dataset, presents an interactive data visualization page. At the top of the page resides a sticky navigation bar offering several selection buttons to the user. A notable facility provided by this application includes a trending prediction feature specifically designed for content creators. By selecting tags related to their video content, creators can predict the optimal time to publish their video to enhance the likelihood of gaining viewership. Additionally, creators can utilize the 'predict' button which triggers a pop-up window. This popup window will show future top 'k' trending tags within the next selected time window (the suitable window size will be determined pre-training) based on a model we trained. The application also boasts a 'classification' feature, providing tag suggestions based on a user-inputted video description. 

The main body of our web application hosts several tables displaying multiple statistical views of the dataset. Located on the left upper corner, we feature a world map, visualizing videos as light data points dispersed globally within a specific time interval. An intriguing feature enables users to click a specific region on the map, extracting data exclusively from that chosen country across all tables. Central to the main body, we offer a table ranking the top 10 trending videos either globally or per country (the ranking algorithm is yet to be confirmed). The lower left section of the application highlights the top 10 trending tags. Clicking on a specific tag triggers a pop-up window displaying trending videos linked to that tag. In the lower center section, we display a tag occurrence graphic, which unveils the frequency of tags in the dataset. The font size is contingent upon the total occurrences of a specific tag, supporting quick visual understanding. Finally, a bar chart is positioned at the lower right corner of the page. This visualization tool aids users in comprehending the overall data dispersion, categorized by time. 

### Work distribution: 

|                                                              | Twinkle            | Advait             | Ronje              | Tamir              |
| ------------------------------------------------------------ | ----------------   | ------------------ | ------------------ | ------------------ |
| Filters                                                      | frontend & backend |                    |                    |                    |
| Search Bar                                                   |                    | frontend & backend |                    |                    |
| Sort Feature                                                 |                    |                    | frontend & backend |                    |
| New Database creation                                        |                    |                    |                    | frontend & backend |

 
