Python Jupyter Notebook
Follow the instructions labelled with 'TODO'

# Overview:

--- DOWNLOAD --------------------------------------------------------------__
Step 0: set up the environment i.e. all filepaths__
Step 1: download the WP and SL data (WP=waypoints, SL=storyline)__

--- PROCESS ---------------------------------------------------------------
Step 2: convert the gzip files to csv                                  
Step 3: move .gz files from 'new' folder to 'gz' folder (as backups; much smaller than csv files)   
Step 4: split the WP csv files into separate days                      

--- UPLOAD ----------------------------------------------------------------
Step 5: upload WP to PostgreSQL database, then delete the WP csv files                                                                                  
Step 6: upload SL to PostgreSQL database, then delete the SL csv files                           
Step 7: run processing pipeline

---------------------------------------------------------------------------

# Folder structure:

MT_MoLe_tmp (root)
├── new_waypoints         (new downloaded waypoints - first as gz, then as csv, then deleted)
├── new_storylines        (new downloaded storylines - first as gz, then as csv,  then deleted)
├── gz_waypoints          (move waypoints gz files here as a backup)
├── gz_storylines         (move storylines gz files here as a backup)
This file
MotionTagConfigKey.txt
C:\...\myDatabasePassword.txt
