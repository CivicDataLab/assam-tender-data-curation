## Assam Tender Data Curation

### Our Goal
We are working closely with the government of Assam to actively identify tenders related to flood preparedness and response. We hope to triangulate this information with other open datasets like satellite imagery, geospatial data, demographic data so that we can build an intelligent data ecosystem to help districts better prepare for floods in Assam. 

### Available Data
We have gathered and standardized tender data for last 5 years of Assam. We are currently working to publish this data in the open, but have shared a private version of the data with you here: 
Link: [CivicDataLab: Assam Public Procurement Data | #not-to-be-shared](https://github.com/CivicDataLab/assam-tender-data-curation/blob/main/data/CivicDataLab_%20Assam%20Public%20Procurement%20Data%20%7C%20%23not-to-be-shared%20-%20ocds_mapped_compiled.csv)

### MetaData
Link to metadata for the above data hhttps://github.com/CivicDataLab/assam-tender-data-curation/blob/main/data/Metadata%20Assam%20Procuremet%20Data.csv

### Recommended Steps
* Design a schema and load this data in a SQL or a no-SQL database and explain us your choice of the database and schema
* Next filter out all the entries related to flood management from this database, you can use the following list of positive(must have) and negative keywords(must not have) to process “tender/externalReference” and “tender/title”:  
   * Positive  keywords: [Flood, Embankment, embkt, Relief, Erosion, SDRF, River, Inundation, Hydrology, Silt, Siltation, Bund, Trench, Drain, Culvert, Sluice, Bridge, Dyke, Storm water drain]
   * Negative keywords: [Driver, Floodlight, Flood Light]
* Among these list of filtered tenders, identify the tenders that have river information present, for example from a “tender/title” : “Immediate measures river Jarasar in pak-5” we need a new field “river/name” : “Jarasar” using an intelligent rule-based engine.
* Compile your database load logic, filtering logic and rule-based engine in a bundle of scripts and share with us over an email or GitHub repository.  

### What are we looking for
* Process: We want to understand your process. How you identified the challenge, and the solution you arrived upon. So documentation of this process would be a valuable addition.
* Skills: Skill-set with respect to designing schema, loading data in database and filtering data.
* Communication: Communication is key in a remote working environment such as ours. We want to observe how you communicate not just through your work but also with us via the various channels we have.

### Timeline
1 week. Do get back to us with any questions and clarifications. 

### How will CDL use the submission?
One of our key values is openness. Our work is  under CC BY 4.0 license and If you choose to, we are happy to exhibit the submission online through our various channels. You are also free to make it part of your portfolio. In case CivicDataLab ends up using any of your work in our live solution(s), we would ensure full disclosure and fair compensation to the creator accordingly.

### Co-creation & Collaboration
At CivicDataLab, we believe in collaboration and co-creation. Feel free to discuss your work with us throughout the given time period either through email or through a scheduled call. We’re more than happy to provide feedback on a continuous basis, and not just at the end of the task. In case you have any questions, don’t hesitate to ping us.
