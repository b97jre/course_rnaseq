# course_rnaseq

This repo contains the course material for NBIS course **Workshop on RNA-Seq**. The rendered view of this repo is available [here](index.html).

## Descriptions

These are descriptions of the files and a guide to updating this repo for course maintainers.

**_site.yml**  
All website configuration options are here. Nothing to be changed here.

**README.md**
You are reading this file now. Nothing to do here.

**index.Rmd**  
This file generates the home page. **Make sure that the date and location is correct**. Verify links.

**schedule.Rmd**  
This file generates the schedule page. **The start time of the course is set to `09:00:00`. Change if needed**.

**schedule.csv**
This table holds the schedule information. Edit in a spreadsheet or text editor. Columns are delimited by `;`. Do not change the number of columns or column names.

*date*: Full date for each day in format dd/mm/yyyy. Missing/empty cells are filled down automatically.  
*room*: Room number for the course. Missing/empty cells are filled down automatically.  
*dur*: Duration for the topic in minutes.  
*topic*: Topic name (Keep it short).  
*person*: Name of the person covering the topic.  
*link_presentation*: (Optional) Link to the presentation. Local links can be just `presentation_topic.html`. Use this labelling convention.  
*link_lab*: (Optional) Link to the lab material. Local links can be just `lab_topic.html`. This is the labelling convention used.  
*link_room*: (Optional) Link to the room location. Can be a google map link, mazemap link etc.  

**lab.Rmd**  
This page brings together all the exercises. Verify links.

**precourse.Rmd**  
This page holds the steps needed to be completed before the course. **Change project ID for each course**.

**info.Rmd**  
This page contains practical information related to the course. **Set location and update info if needed**.

**presentation_topic.Rmd**  
RMarkdown presentation files for various topics. Replace 'topic' with a short name of the topic.  

**lab_topic.Rmd**
RMarkdown lab files for various topics. Replace 'topic' with a short name of the topic.  

## Rendering

The website is rendered by running `rmarkdown::render_site()` in the project directory. This generates the HTML files and all other necessary files and moves it into a directory named `docs`. Open `docs/index.html` to start. This is convenient when moving the contents to a GitHub repo as the docs directory can be set as the Github pages.

For testing purposes, you can run `rmarkdown::render("lab_topic.Rmd")` on individual Rmd files. 

---

**2019** NBIS | SciLifeLab