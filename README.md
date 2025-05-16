*UCSB MEDS* - *EDS 213 - Database Management*


# Final Project - Finding America's Favorite National Park

![R Programming](https://img.shields.io/badge/R_Programming-cornflowerblue?style=for-the-badge&logo=R) ![SQL](https://img.shields.io/badge/SQL-purple?style=for-the-badge)  ![UCSB MEDS](https://img.shields.io/badge/UCSB%20MEDS-blue?style=for-the-badge) 

**Author:** Nicole Pepper

<div style="text-align: left;">
  <img src="https://github.com/nicolelpepper/eds213-nps-project/blob/main/images/smnp.jpg" alt="Image" width="900">

*Image by [Bryson City]([https://unsplash.com/photos/aerial-photography-of-white-frames-on-top-of-water-eUfnha6ev9g](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.explorebrysoncity.com%2Fthings-to-do%2Fgreat-smoky-mountains-national-park%2F&psig=AOvVaw3q7BvdR_njsJ5BcTdUlWuo&ust=1747442266861000&source=images&cd=vfe&opi=89978449&ved=0CBQQjRxqFwoTCLC6mO7fpo0DFQAAAAAdAAAAABAE))*

### About the Repo:
[This repository](https://github.com/nicolelpepper/eds213-nps-project) contains Quarto Markdown documents of my R analysis Finding America's Favorite National Park. For this analysis, I used SQL in R-Studio to clean, merge, and rearrange datasets from the National Park Service into a duck db databse for National Parks popularity.

### Technical Highlights:
- Programming in R
-  Querying in SQL
- Data visualization with `ggplot`

### Data Descriptions:

- The `species` data is a record of species observations at National Parks from the NPS Biodiversity Dataset. This data was used to assess how popular parks are for different wildlife species. The data is from the NPS, however I accessed it from a [Tidy Tuesday Repo](https://github.com/frankiethull/NPSpecies). The data is stored in `/data/raw` folder in the repo as `species.rda`.
  
- The `parks` dataset is from the National Parks Service. It contains information on National Parks. The data is from the NPS, however I accessed it from a [Tidy Tuesday Repo](https://github.com/frankiethull/NPSpecies). The data is stored in `/data/raw` folder in the repo as `parks.rda`.
    
- The `visitation` dataset is from the National Parks Service. This data was used to assess how popular a park is based on their annual visitation rates. I accessed it from their [Visitor Use Statistics Dashboard](https://www.nps.gov/subjects/socialscience/visitor-use-statistics-dashboard.htm). The data is stored in `/data/raw` folder in the repo as `park-visitation.csv`.

- `national_parks.duckdb` is the final relational database that I created for this project. It is stored in the `/data/clean` folder.

**Overview of database structure:**
 <div style="text-align: left;">
  <img src="https://github.com/nicolelpepper/eds213-nps-project/blob/main/images/db-diagram.png" alt="Image" width="900">

**Other Files:**
- `dependencies` A list of the the dependencies and environment requirements used for this analysis are listed in the `dependencies.txt` file.
- `data cleaning` The data cleaning for this project is located in the file called `NPS_Data_Prep.qmd`
- `query` & `visualization` The sql query and visualization for this project are located in the file called `NPS_Query.qmd`

### Repo structure:

```
eds213-nps-project
├── NPS_Data_Prep.qmd
├── NPS_Query.html
├── NPS_Query.qmd
├── NPS_Query_files
├── README.md
├── data
│   ├── clean
│   │   ├── national_parks.duckdb
│   │   └── national_parks_analysis.duckdb
│   └── raw
│       ├── park-visitation.csv
│       ├── parks.rda
│       └── species.rda
├── dependencies.txt
├── eds213-nps-project.Rproj
└── images
    └── smnp.jpg
```

### References:
National Park Service. NPS Biodiversity Database. U.S. Department of the Interior. Retrieved May 2025, from [https://irma.nps.gov/NPSpecies/](https://github.com/frankiethull/NPSpecies)

National Park Service. Visitor Use Statistics Dashboard. U.S. Department of the Interior. Retrieved May 2025, from https://www.nps.gov/subjects/socialscience/visitor-use-statistics-dashboard.htm

