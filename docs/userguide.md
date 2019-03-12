# GEONEX Concepts

- GEONEX Account - You need to create it to get access to GEONEX resources, including AWS EC2 instances, repos, containers, tasks and buckets.
- Buckets - AWS S3 buckets, used as input and output storage of GEONEX products. The geonex algorithm pools has different algorithms based on GEONEX datasets. The dataset category enables to display the latest ready datasets for downloading or used by scientists. NOAA GOES-16 and GOES-17 have been trackable real-time and Himawari8 is semi real-time.
- Repos - a dockerized image, within it a combination of a file system and GEO application was built. It can be hosted on public docker registry services ([hub.docker](https://hub.docker.com/); [AWS ECR](https://aws.amazon.com/ecr/); [gcr.io](https://cloud.google.com/container-registry/))
- Containers - a standard unit on GEONEX approved by the administrator to finish specific processing/analysis jobs. User enable to see all running, stopped, or finished tasks in the dashboard. Some user with permission also can view products from the specific tasks, and check log files for each task. These tasks are automatically executed at the back-end using EC2 instances. User can also customize the instances with different  types and sizes for running each container.
- Tasks - the runtime instance of a GEONEX containers (repo).
- Workspace  - containers related to specific output buckets, which can be browsed in the viewer









# Policies

After registering their images, guest user opens GEONEX Images tab, and clicks “ Request” button. The dashboard will automatically send an email notification to system administrator, and let him/her know there is one image need him/her approve. Administrator logins the dashboard and clicks “Approve” button, then finish the approval. 

## AWS EC2 instance