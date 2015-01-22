# Objective
The objective of the project is to create a knowledge-base for clinical conditions. 
Input :  Unstructured text ( medical articles, health data , patient data from KAggle, social media data from FB and Twitter etc) 
Outpt: To find the various entities ( diseases, disorders, signs, symptoms, procedures and drugs) that have been discussed in each document.  Then create a visualization (using d3.js or neo4j) to visualize the inerations between 
           various data states. 
Some of the questions that we can address are (a) based on given information, what are the drugs that are most popular for a disease ? (b) if two drugs are prescribed for the same disease, which one is more effective ? 
--------------------------------------------------------------------------------------
Phase 1 :  (Downloading and preprocessing )
   Here , I will be downloading the data from various sources ( mostly from open access journals in different formats; pdf , doc, docx, html, rtf, xml )  into Amazon S3
  Use APache Tika or Apache POI to parse the text data. 
  Move the parsed data into a NoSQL database (HBASE) using SQOOP 
Phase 2: Analytics 
  Here I plan to do some analytics based on NLP (natural language processing libraries and ML (machine learning, Mahout) tools inside he Hadoop framework. 
Phase 3: Visualization
   uisng graph-daabase visualizaions ( d3.jas or neo.4j) . It would look something like this : 
   http://lenovodev.com/blog/tech-modder/2014/02/18/graphs-databases-and-just-hint-of-sage/#.VL_9WXuNmPU  
   Except, instead of Matrix characters, I plan to put symptoms, diseases, drugs etc and their interactions. 


