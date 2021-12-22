# Movies-ETL
## Project Overview
After assisting Amazing Prime with extracting, transforming, and loading a set of clean movie data for their upcoming Hackathon event, our next tesk was to provide Amazing Prime with a tool to keep the dataset up to date. In this project we created an automated pipeline that can take in new data, perform the appropriate transformations, and load the data into existing tables.

## Results 
#### Deliverable 1
- The pipeline begins with a function that reads in our three data files and creates three separate DataFrames.
<img width="700" alt="Extract" src="https://user-images.githubusercontent.com/93271297/147161163-4986a505-2556-4f97-a19b-fa71df689714.png">

#### Deliverable 2
- Tansformed Wikipedia data in order to merge it with the Kaggle metadata
  - Filtered out TV Shows 
  - Cleaned values in box office, budget, release date, and running time columns

#### Deliverable 3
- Transformed Kaggle metadata and MovieLens rating data and converted the transformed data into separate DataFrames 
- Merged the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create a new **movies_df** DataFrame 
- Merged the MovieLens rating data DataFrame with the movies_df DataFrame to create a **movies_with_ratings_df** DataFrame

#### Deliverable 4
- Added the final movies_df DataFrame and the MovieLens rating csv data to a SQL database 
- Performed query to confirm data transfer
<img width="688" alt="df_to_DB" src="https://user-images.githubusercontent.com/93271297/147163385-58fbffad-d0b4-4c0f-bd41-e2d4dc97730e.png">
<img width="688" alt="movies_query" src="https://user-images.githubusercontent.com/93271297/147163644-bdda2a0c-c07a-4e3d-b929-737df18a1636.png">

