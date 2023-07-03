# Swiggy-Restrauant-Recommendation-Model

**--Introduction--**

As it becomes crucial for customers at a new location to find the appropriate restaurant based on their preferences so a recommendation model can be a handful for the customers to get what they want and also for the companies to the betterment of services for their further future growth.

**--Problem Aimed to Solve--**

To develop a Swiggy restaurant recommender model which can predict the suitable restaurant, price for two, and dish name based on a budget price, cuisine, and location 

**--Data Description--**

1. EXCEL FILES: This folder contains 3 Excel files where
a. swiggy_table1 has the link of the restaurant, name of the restaurant, cuisine, price for 2 customers, and rating of the restaurants in .csv format.
b. swiggy_table2 has the dish price, total rating numbers, dish name, dish category, and name of the restaurants.
c. finalized_swiggy_dataset has the combined two tables mentioned above and the final dashboard based on this.

2. Jupiter notebook files: This folder has 3 files where
a. web_scrapping has the Jupiter files which were used to scrap the data from Swiggy(Bangaluru)
b. ml2 file was used to clean the dataset after extraction and to convert the HTML restaurant details into CSV files.
c. swiggy_model file contains the code to create an algorithm to predict the restaurant name, the price for two, and the dish name based on the budget price, cuisine, and location.

3. restaurant_recommender folder has the source code file which we used to show our model on the HTML webpage.
 
**--Methodolgy--**

The project involves extracting, collecting, and processing Swiggy restaurants' data and then utilizes data analysis techniques and machine learning modeling to predict the final output based on the preferences.

**--Phases--**

![Screenshot 2023-07-01 074157](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/46949c29-50ad-47c3-a6b2-41b0dfd480a9)

--Scrapping the data--

![Screenshot 2023-07-01 175036](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/56bea6f7-ecaa-463f-91f7-34278f7f1161)

![Screenshot 2023-07-01 175110](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/b04b98f6-7401-4a80-be72-b931a52c9cf1)

![Screenshot 2023-07-01 182526](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/604b39ef-e077-40a5-b9b7-ba9d23673044)


1. To scrap the data from the Swiggy web page for Bengaluru restaurants, beautiful soup, and html5lib were used. The data extracted was in HTML format at first and classes of different objects were used to fetch the details.

![Screenshot 2023-07-01 175139](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/b6dd9b8b-7d16-4f06-a131-774c7ba51d74)

2. After we convert the html data into some useful tabular data in CSV format, it was looking something like this having a lot of noise.
   
 ![Screenshot 2023-07-01 181745](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/14291b6e-5dd1-4f73-ba35-b478a1d02382)

3. Panda was used to handle the null values, change the data types, and manipulate the data.
   
![Screenshot 2023-07-01 175213](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/b8cc3a90-6cce-4905-bf01-bf2d28bd354a)

4. This is what the cleaned data was looking like.

**--Machine Learning Model--**

![Screenshot 2023-07-01 183325](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/54f6f9db-39b6-4f0b-b09a-993f974e3807)

![Screenshot 2023-07-01 183408](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/18d8423a-2257-4c54-b8ca-f5abe4be36b9)


**--HTML web page for Restaurants Recommender--**

![Screenshot 2023-07-03 231118](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/cb14877c-eb66-4a33-b054-82bf07c47a7b)

**--HTML Flask code**

![Screenshot 2023-07-03 231159](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/841a1347-3fb3-4931-b8c9-048aed3060a4)


**--DashBoard Creation--**

Here is the main dashboard which is dynamic in nature and the slicer added is for different locations, cuisine, and restaurant name.

![Screenshot 2023-07-01 074506](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/34978159-7882-4108-9566-806a7c07d06d)


**--Insights--**

Through Excel DashBoard, the project represents some valuable insights in a visually engaging manner, using charts, graphs, and slicers. These visual representations help to show the trend for different locations, and cuisine, enabling customers/decision makers to make well-informed decisions.

1.
![Screenshot 2023-07-01 074900](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/94aae878-c92f-4741-9241-7b2178927e2d)

Here are the top 3 locations having the number of restaurants with corresponding ratings. By looking at the chart one can conclude that Koramangala has the highest-rated restaurants among all 3.

2.
![Screenshot 2023-07-01 075050](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/21bc9504-82bc-4bd5-b072-557cfa1f99a1)

Here is the chart that represents the number of restaurants at different locations in Bangalore. As it can be concluded that Koramangala, Indiranagar, and Jayanagar have the highest number of restaurants.

3.
![Screenshot 2023-07-01 075554](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/2149868b-322a-4f99-88c7-55542335be1b)

Here are the details of the cuisineS at top locations in Bangalore.

4.
![Screenshot 2023-07-01 075750](https://github.com/Ashish23-Karn/Swiggy-Restrauant-Recommendation-Model/assets/121361369/ea195c4f-5d4a-4458-891b-444c11ad2a7a)

Here are some dishes with higher prices being served in Bangalore, one can conclude that the "butter naan combo" dish has the highest price for all.

**--Challenges and learnings--**

1. The main challenge posed by this project was to create a webpage by using HTML to show our model.
2. Another challenge posed by this project was to scrape the data from the Swiggy website at first, cleaned it as there was a lot of noise in the data and redundant values as well, then by choosing the appropriate ml algorithm to predict correctly.
3. As all of our team members are working professionals, we were finding difficulty in managing time and the time availability of each team member is different. Firstly, we brainstormed and formed a flowchart of works that helped us be on track. We allocated the work according to each person’s time availability and task priority

   --Overall, The project/model can serve as a handful restaurant locator for the general public and the dashboard can help the decision-makers of the company to improve services and further growth. 
