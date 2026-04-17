# Day 4 

# S3 Storage Classes 

S3 can host static website accessible to the internet. 

INTRO TO S3
* S3 versioning:
Amazon S3 allows you to enable versioning at the bucket level .
* This helps safeguard your data by managing file versions effectively. 


S3 REPLICATION 
* Cross-Region Replication (CRR) copies objects between buckets in different AWS Regions.

* Same-Region Replication (SRR) copies objects between buckets within the same AWS Region.


S3 Storage Classes:
* Amazon S3 Standard - General Purpose
* Amazon S3 Standard - Infrequent Access (IA)
* Amazon S3 Intelligent Tiering
Amazon S3 One Zone - Infrequent Access
* Amazon S3 Glacier Instant Retrieval
* Amazon S3 Glacier Flexible Retrieval
* Amazon S3 Glacier Deep Archive


S3 Standard - General Purpose
* It offers 99.99% availability for highly accessed data .
* It basically ideal for big data analytics, mobile apps , gaming.


S3 Infrequent Classes
* S3 Standard- Infrequent Access (Standard -IA):
       
       * It is basically suitable for backups and disaster recovery.


* S3 one zone -Infrequent Access (One Zone-IA)

       * It provided 99.5% availability.


S3 GLACIER CLASSES:
It is basically low cost storage meant for archiving and for backup.

It take your price for storage and object retrieval cost .

* Amazon S3 Glacier Instant Retrival
        
        * Millisecond Retrieval
        * minimum storage for around 90 days.

* Amazon S3 Glacier Flexible Retrival
        * It also take minimum storage duration of 90 days.

* Amazon S3 Glacier Deep Archive 
        * It is basically for the long term storage.

        * and minimum storage for around 180 days.
