## Hadoop, do we still need it?

Hadoop, the main name in bigdata and data analytics world, was founded in the late of 2006 by Yahoo as a new era in all data topics such as data seinces and data structure. Hadoop is an open sources platform for distributed storage and distributed processing thats targiting bigdata processing. In that time (2006), the term of "BigData" was still new to the data world thats the contemporary data tools was unable to obsorbing the daily bigdata in all of structured, semi-structured and non-structured faces.

The term of "Distributed" means that hadoop is running over a hundreds but thousends of machines, this structure will dollout the workload between the nodes, and also an easy hardware replacment once needed. Thus, Hadoop got a solid based to getting started in bigdata era and shortly become the master in this topic. Hadoop can treats many kind and resources of data due to its running over a bunch of ecosystems, such as HDFS (Hadoop distributed file system), MapReduce, YARN, Hive, Sqoop, Pig, Flume, Spark and all the rest. However, each one of these ecosystems is directed to a specific job in data analysis.

HDFS, is Hadoop file system used to store data.
MapReduce is for disributing processing (Batch Processing)-Slow
YARN is for resource management
Spark is for distributing processing (In memory processing)-Fast
Hive is for structured data "SQL" and its Hive name "HQL"
Sqoop and Flume are both for data injection.

Since that time till now, there were many ecosystems was developed and pushed to work under Hadoop umbrella such as Storm, Ranger, and Spark2. However, to run hadoop in a best practice, you have to build a cluster, actually, a huge cluster running one Namenode and thousends of Datanodes are all running on premise. 

So, by now we got understand about Hadoop importance in data analytics world and the uses of most common ecosystems in the cluster. Hadoop must be available at anytime its required to fetch some info from the cluster; the challenge start begins when the on primes cluster required a lot of maintenance services and hardware replacement to keep the cluster up and running. The second challenge is came from the cluster it self in a term of "Big data in small files". As metionaned earlier in this parigraph, Hadoop must be available to insight any required information at anytime. 

The first cluster limitation is the "on primise running or local installation". The local machines are physical resources with a fixed running ability thats if the one machine is Core i7 with 32 Gb RAM and 1 TB SSD, it will remain as is unless someone update it phisycally,so if this machine is datanode, its not a problem to switch it off, upgrade, then back to work, but if its a Namenode, the upgrade will be more complicated due to the Namenode BK "Secondary Namenode" must be updated to takeover till the Namenode maintenaince has been done. But all by all, the cluster is under availablity risk due to several factors such as power supply, Hardware failuer, OS/Connection down and so on.\

One more major limitation of Hadoop is the batch processing, in other words "Mapreduce". Mapreduce is the computing and processing side of hadoop, its the ecosystem whom responsable of dolling out the big task into some small tasks over the Datanodes. As its name "Map+Reduce", it will start by the Jobtracker resident in the Namenode whom recive the analytic job then doll out it to the recivers in the Datanodes called Task traker, this is what we call it "Map". the second mession is collecting the results from all task trackers and show the final insghts to the user, this taask called reduce. Wow thats looks great, but it eas in the last 2010 when you create the task, go get some coffee and relax, then come back to check the results, but now in 2021 it dosent work any more, the management layer are looking for "At once information" which is cant be supported with Mapreduce and HDFS.

Something more, the cloud services. Since the raise of cloud services such as AWS and Azure, Azure used to grab Hadoop as an open source system and transform it to be HDInsights only as a cloud service, and same story with Amazon. Thus, why you need to build a Hadoop cluster in your plac with all the risks we maintioned them already, but you can just wizard a better cluster on the cloud?


## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/mbmasadeh/HadoopNeed/edit/main/docs/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/mbmasadeh/HadoopNeed/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
