# On-Semiconductor APAC Data Migration/Configuration

## Project Outline

**Short Description:**
 An implementation that migrates orion data to the APAC region instance to display user metrics. View:*Notes.txt* for more detail.
 
**Author**  [AJ Brown](https://github.com/AJ-Brown-InTech) / Loop1, LLC

**Client** ON Semiconductor 

## Configuration

**Installation**
1. Download and install Python from [this link](https://nodejs.org/en/download/)
2. Install [Git for Windows](https://gitforwindows.org/) to make updating the project with any future code easier
3. From a command prompt, `git clone https://github.com/aj-brown-loop1/Onsemiconductor-APAC_data_migration-nodejs.git` where the project will live and be updated if changed
4. Create a configuration file as described below
5. Navigate to the project folder with command line and run `python main.py`

Application expects config files named `old.yaml` & `new.yaml` stored in the same directory as main.py This code can be used as a template:

```
Old.yaml
server:  "server-name"
port: port-number
user : "orion-username"
password:  "orion-password"

New.yaml
server:  "server-name"
port: port-number
user : "orion-username"
password:  "orion-password"

```

**Descriptiom of Configuration Fields:**
* **runFreq:**  how often (in minutes) the script will check for new Audit events in both DocuSign and Web Help Desk. This script will listen constantly for these requests when running.
* **accountId:**  numerical ID from DocuSign to permit access rights to the api. This can be found under Settings > Apps and Keys in DocuSign Developer Account. The ID is part of the RESTAPI Calls.

# delete-for-onsemi-once-updated
