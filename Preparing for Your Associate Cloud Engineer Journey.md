
# <p align="center">Setting Up a Cloud Solution Environment:</p>
<h1>Diagnostic Questions.</h1>

Question.   The Operations Department at Cymbal Superstore wants to provide managers access to information about VM usage without allowing them to make changes that would affect the state. You assign them the Compute Engine Viewer role. Which two permissions will they receive?/n
Answer.     compute.images.list, compute.images.get

Question.   Pick two choices, from the options below, that provide a command line interface to Google Cloud.
Answer.     Cloud Shell, Cloud SDK

Question.   Stella is a new member of a team in your company who has been put in charge of monitoring VM instances in the organization. Stella will need the required permissions to perform this role. How should you grant her those permissions?
Answer.     Add Stella to a Google Group in your organization. Bind that group to roles/compute.viewer.

Question.   You need to add new groups of employees in Cymbal Superstore’s production environment. You need to consider Google’s recommendation of using least privilege. What should you do?
Answer.     Grant predefined and custom roles that provide necessary permissions and grant basic roles only where needed.

Question.   How are billing accounts applied to projects in Google Cloud? (Pick two).
Answer.     A project and its resources can only be tied to one billing account.
            A billing account can be linked to one or more projects.
           
Question.   How are resource hierarchies organized in Google Cloud?
Answer.     Organization, Folder, Project, Resource

Question.   What Google Cloud project attributes can be changed?
Answer.     The Project Name.

Question.   You want to use the Cloud Shell to copy files to your Cloud Storage bucket. Which Cloud SDK command should you use?
Answer.     gsutil

Question.   Jane will manage objects in Cloud Storage for the Cymbal Superstore. She needs to have access to the proper permissions for every project across the organization. What should you do?
Answer.     Add Jane to a group that has the roles/storage.objectAdmin role assigned at the organizational level.

Question.   Fiona is the billing administrator for the project associated with Cymbal Superstore’s eCommerce application. Jeffrey, the marketing department lead, wants to receive emails related to budget alerts. Jeffrey should have access to no additional billing information. What should you do?
Answer.     Use Cloud Monitoring notification channels to send Jeffrey an email alert.



<h1>Knowledge Check Quiz:</h1>

Question.   What is the lowest level basic role that gives you permissions to change resource state?
Answer.     Editor.

Question.   Which Google Cloud interface allows for scripting actions in a set of command line executables?
Answer.     Cloud Shell.


<h1>Plannning and Configuring a Cloud Solution:</h1>

Diagnostic Quiz:

Question.    You want to deploy a microservices application. You need full control of how you manage containers, reliability, and autoscaling, but don’t want or need to manage the control plane. Which compute option should you use?
Answer.      Google Kubernetes Engine

Question.    Cymbal Superstore has a need to populate visual dashboards with historical time-based data. This is an analytical use-case. Which two storage solutions could they use? https://cloud.google.com/bigtable/docs/overview#other-storage-options
Answer.      BigQuery, Cloud Bigtable

Question.    The projected amount of cloud storage required for Cymbal Superstore to enable users to post pictures for project reviews is 10 TB of immediate access storage in the US and 30 TB of storage for historical posts in a bucket located near Cymbal Superstore’s headquarters. The contents of this bucket will need to be accessed once every 30 days. You want to estimate the cost of these storage resources to ensure this is economically feasible. What should you do?
Answer.      Use the pricing calculator to estimate the price for 10 TB of multi-region Standard storage, 30 TB for regional Nearline, and egress charges for reads from the bucket.

Question.    Cymbal Superstore decides to migrate their supply chain application to Google Cloud. You need to configure specific operating system dependencies. What should you do?
Answer.      Implement an application using virtual machines on Compute Engine.

Question.    Cymbal Superstore’s supply chain application frequently analyzes large amounts of data to inform business processes and operational dashboards. What storage class would make sense for this use case?
Answer.      Standard

Question.    Cymbal Superstore needs to analyze whether they met quarterly sales projections. Analysts assigned to run this query are familiar with SQL. What data solution should they implement?
Answer.      BigQuery

Question.    Cymbal Superstore is piloting an update to its ecommerce app for the flagship store in Minneapolis, Minnesota. The app is implemented as a three-tier web service with traffic originating from the local area and resources dedicated for it in us-central1. You need to configure a secure, low-cost network load-balancing architecture for it. How do you proceed?
Answer.      Configure a standard tier proxied external https load balancer connected to the web tier as a frontend and a regional internal load balancer between the web tier and the backend.

Question.    Which Google Cloud load balancing option runs at Layer 7 of the TCP stack?
Answer.      Global http(s)

Question.    An application running on a highly-customized version of Ubuntu needs to be migrated to Google Cloud. You need to do this in the least amount of time with minimal code changes. How should you proceed?
Answer.      Create Compute Engine Virtual Machines and migrate the app to that infrastructure

Question.    Cymbal Superstore decides to pilot a cloud application for their point of sale system in their flagship store. You want to focus on code and develop your solution quickly, and you want your code to be portable. How do you proceed?
Answer.      Package your code to a container image and post it to Cloud Run.


Knowledge Check:

Question.    Which storage class is designed for long term storage has a 365 day minimum storage agreement, and a lower storage price as compared to other storage types?
Answer.      Archive storage

Question.    Which serverless option is based on developing and executing small snippets of code?
Answer.      Cloud Functions



<h1>Deploying and Implementing a Cloud Solution:</h1>

Diagnotic Quiz:

Question.    You need to analyze and act on files being added to a Cloud Storage bucket. Your programming team is proficient in Python. The analysis you need to do takes at most 5 minutes. You implement a Cloud Function to accomplish your processing and specify a trigger resource pointing to your bucket. How should you configure the --trigger-event parameter using gcloud?
Answer.      --trigger-event google.storage.object.finalize

Question.    Cymbal Superstore asks you to implement Cloud SQL as a database backend to their supply chain application. You want to configure automatic failover in case of a zone outage. You decide to use the gcloud sql instances create command set to accomplish this. Which gcloud command line argument is required to configure the stated failover capability as you create the required instances?
Answer.      --availability-type

Question.    You need to quickly deploy a containerized web application on Google Cloud. You know the services you want to be exposed. You do not want to manage infrastructure. You only want to pay when requests are being handled and need support for custom packages. What technology meets these needs?
Answer.      Cloud Run

Question.    Cymbal Superstore’s sales department has a medium-sized MySQL database. This database includes user-defined functions and is used internally by the marketing department at Cymbal Superstore HQ. The sales department asks you to migrate the database to Google Cloud in the most timely and economical way. What should you do?
Answer.      Configure a Compute Engine VM with an N2 machine type, install MySQL, and restore your data to the new instance.

Question.    The backend of Cymbal Superstore’s e-commerce system consists of managed instance groups. You need to update the operating system of the instances in an automated way using minimal resources. What do you do?
Answer.      Create a new instance template, then click Update VMs. Set the update type to PROACTIVE. Click Start.

Question.    What action does the terraform apply command perform?
Answer.      Sets up resources requested in the terraform config file.

Question.    You require a Cloud Storage bucket serving users in New York City. There is a need for geo-redundancy. You do not plan on using ACLs. What CLI command do you use?
Answer.      Run a gsutil mb command specifying a dual-region bucket and an option to turn ACL evaluation off.

Question.    Which Virtual Private Cloud (VPC) network type allows you to fully control IP ranges and the definition of regional subnets?
Answer.      Custom mode network

Question.    The development team for the supply chain project is ready to start building their new cloud app using a small Kubernetes cluster for the pilot. The cluster should only be available to team members and does not need to be highly available. The developers also need the ability to change the cluster architecture as they deploy new capabilities. How would you implement this?
Answer.      Implement a private standard zonal cluster in us-central1-a with a default pool and an Ubuntu image.

Question.    Cymbal Superstore’s marketing department needs to load some slowly changing data into BigQuery. The data arrives hourly in a Cloud Storage bucket. You want to minimize cost and implement this in the fewest steps. What should you do?
Answer.      Use the BigQuery data transfer service to schedule a transfer between your bucket and BigQuery.


Knowledge Check:

Question.    Which services are based on logic implemented in containers? (Pick two).
Answer.      Cloud Run
             Google Kubernetes Engine
             
Question.    Which data storage service is a unique globally available, horizontally scalable database with relational semantics?
Answer.      Cloud Spanner


<h1>Ensuring Successful Operation of a Cloud Solution:</h1>

Question.    You have a scheduled snapshot you are trying to delete, but the operation returns an error. What should you do to resolve this problem?
Answer.      Detach the snapshot schedule before deleting it.

Question.    You want to view a description of your available snapshots using the command line interface (CLI). What gcloud command should you use?
Answer.      gcloud compute snapshots list

Question.    What is the declarative way to initialize and update Kubernetes objects?
Answer.      kubectl apply

Question.    What Kubernetes object provides access to logic running in your cluster via endpoints that you define?
Answer.      Services

Question.    Cymbal Superstore’s GKE cluster requires an internal http(s) load balancer. You are creating the configuration files required for this resource. What is the proper setting for this scenario?
Answer.      Annotate your service object with a neg reference.

Question.    Cymbal Superstore has a subnetwork called mysubnet with an IP range of 10.1.2.0/24. You need to expand this subnet to include enough IP addresses for at most 2000 new users or devices. What should you do?
Answer.      gcloud compute networks subnets expand-ip-range mysubnet --region us-central1 --prefix-length 21

Question.    You want to implement a lifecycle rule that changes your storage type from standard to nearline after a specific date. What conditions should you use? (Pick two).
Answer.      CreatedBefore
             MatchesStorageClass
             
Question.    Which of the following tasks are part of the process when configuring a managed instance group? (Pick two).
Answer.      Defining Health checks
             Providing Number of instances

Question.    You have a Cloud Run service with a database backend. You want to limit the number of connections to your database. What should you do?
Answer.      Set Max instances.

Question.    Cymbal Superstore’s supply chain management system has been deployed and is working well. You are tasked with monitoring the system’s resources so you can react quickly to any problems. You want to ensure the CPU usage of each of your Compute Engine instances in us-central1 remains below 60%. You want an incident created if it exceeds this value for 5 minutes. You need to configure the proper alerting policy for this scenario. What should you do?
Answer.      Choose resource type of VM instance and metric of CPU utilization, condition trigger if any time series violates, condition is above, threshold is .60 for 5 minutes.


Knowledge Check:

Question:    Which Cloud Run autoscaling setting should you set if you want to limit cost?
Answer:      Max instances

Question:    What GKE object implements an http(s) load balancer?
Answer:      Ingress


Configuring and Access and Security:

Diagnostic Quiz:

Question.    Cymbal Superstore is implementing a mobile app for end users to track deliveries that are en route to them. The app needs to access data about truck location from Pub/Sub using Google recommended practices. What kind of credentials should you use?
Answer.      Service account key

Question.    You are trying to assign roles to the dev and prod projects of Cymbal Superstore’s e-commerce app but are receiving an error when you try to run set-iam policy. The projects are organized into an ecommerce folder in the Cymbal Superstore organizational hierarchy. You want to follow best practices for the permissions you need while respecting the practice of least privilege. What should you do?
Answer.      Ask your administrator for the roles/resourcemanager.folderIamAdmin for the ecommerce folder

Question.    Which Cloud Audit log is disabled by default with a few exceptions?
Answer.      Data Access audit logs

Question.    Outline where Cloud Audit logs can be accessed: in the logging tab of the operations interface Link: https://cloud.google.com/storage/docs/audit-logging You are configuring audit logging for Cloud Storage. You want to know when objects are added to a bucket. Which type of audit log entry should you monitor?
Answer.      DATA_WRITE log entries

Question.    You have a custom role implemented for administration of the dev/test environment for Cymbal Superstore’s transportation management application. You are developing a pilot to use Cloud Run instead of Cloud Functions. You want to ensure your administrators have the correct access to the new resources. What should you do?
Answer.      Make the change to the custom role locally and run an update on the custom role

Question.    Which of the scenarios below is an example of a situation where you should use a service account?
Answer.      For individual GKE pods

Question.    You need to configure access to Cloud Spanner from the GKE cluster that is supporting Cymbal Superstore’s ecommerce microservices application. You want to specify an account type to set the proper permissions. What should you do?
Answer.      Assign permissions through service account referenced by the application



Knowledge Check:

Question.   You are authenticating an application to service APIs. Both resources are internal to the Google Cloud environment. What type of credentials should you use?
Answer.     Temporary credentials

Question.    What kind of account is meant for machine-to-machine communication in Google Cloud?
Answer       Service account


