Purpose: download storyline and/or waypoint data from MT platform. Optional: process data and upload to a PostgreSQL database.<br/>
Python Jupyter Notebook. Follow the instructions labelled with 'TODO'

## Overview:

#### Download <br/>
Step 0: set up the environment i.e. all filepaths <br/>
Step 1: download the WP and SL data (WP=waypoints, SL=storyline)

#### Process  <br/>
Step 2: convert the gzip files to csv                                       <br/>
Step 3: move .gz files from 'new' folder to 'gz' folder (as backups; much smaller than csv files) <br/>
Step 4: split the WP csv files into separate days                           <br/>

#### Upload br/>
Step 5: upload WP to PostgreSQL database, then delete the WP csv files     <br/>
Step 6: upload SL to PostgreSQL database, then delete the SL csv files     <br/>
Step 7: run processing pipeline                                            <br/>

## Folder structure:

MT_MoLe_tmp (root)       <br/>
├── new_waypoints         (new downloaded waypoints - first as gz, then as csv, then deleted) <br/>
├── new_storylines        (new downloaded storylines - first as gz, then as csv,  then deleted) <br/>
├── gz_waypoints          (move waypoints gz files here as a backup) <br/>
├── gz_storylines         (move storylines gz files here as a backup) <br/>
This file <br/>
MotionTagConfigKey.txt <br/>
C:\...\myDatabasePassword.txt
