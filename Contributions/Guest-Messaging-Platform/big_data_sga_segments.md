# Standard Guest Attribute Segments

## Description 

As part of the migration from Big Red 2 (BR2) to Big Red 3 (BR3), it was necessary for our team to 
create guest audience segments so that marketing planners are able to efficiently tailor certain content to specific groups
of Target guests. The goal of creating these Standard Guest Attribute Segments (SGA Segments) was to drive guest engagement
with our email and push marketing campaigns so that we can see increase performance and revenue from our marketing streams. 

Some business requirements for creating these SGA segments included the following:
- Segments had to based on 60 days of browse and 120 days of sales data
- All guests had to be opt-in and labeled as "marketable" by our source datasets
- Segments have to be platform specific by push and email channel
- Segments need to be refreshed on a daily basis

To meet these requirements, a new Apache spark job had to be created and configured to run everyday overnight and to cache the list of audience 
segments in a MongoDB. Info on the location and size of these segments were to be made accessible through Composer UI 

The tech stack for this story was Scala, SQL, Apache Spark, Hadoop, MongoDB, BigRed3, Hyperion, and Dataminer. 


## Noteworthy Tasks

- Constructed a new Apache Spark job that could read millions of rows of guest browse, sales, and marketing data so that Morpheus could
market specific content to certain segments of Target guests.
- Refined the above Apache Spark job to be configurable via YAML file so that Morpheus is able to make new SGA segments without doing major 
code changes.
- Configure the SGA spark job to take into account common emergency situations in case of failure to create or update certain 
SGA segments in production
- Engaged in detailed validation and audit of SGA segments with Morpheus business partners to ensure the highest quality and trust in the new updated
audience segments.

## Learnings

- Strengthened my skills creating service, adapter, connector, and model classes in Scala Programming Language 

- Forged my skills working with "Big Data" technologies like Scala, XML, Apache Spark and Hadoop as well as Target's Hyperion UI Tool
- Attained higher knowledge building complex SQL queries while validating the size and quality of new SGA segments. 
 

## Screenshots
*Due to the internal nature of this project, screenshots and some relevant links were redacted* 
