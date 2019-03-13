## Get Started 

This article will guide you through your first steps in GeoNEX dashbard. You'll be working with some sample data from [GOES16](https://registry.opendata.aws/noaa-goes/). You'll see examples of a wildfire real-time detection using GeoNEX.





In Part 1, you'll learn how to:



- submit an algorithm
- request a cloud runner 
- retrieve geostationary data from AWS S3 bucket
- check the outputs of algorithm as well as the runtime log



In Part 2, you'll learn how to:

- create visualization & analytics code for your outputs
- run the code in the notebook
- share your results with others



### How to register docker image?

The docker image could come from one public docker hub, where user can directly download it without any permissions. User have to put image’s source, description, user name, email, and user’s organization  when registering your image. Once you register the image, the image can be found in NEX Repositories like below:

![img](/Users/jxiong1/Desktop/GHI/geonex-doc/docs/assets/wf2B6e195WerE4RuvEPfzy050_mgncjL_NUHyRlSN3ouTU8RUUygPDyWVHurnrcPX958M_t-rXmSfjfhUvk_lUe4hhtXVh4Lbd5yY1HgVW7SJnpSs40PQ2wrLQH-0M6PJc8a_oNl.png)

For each image, user can execute “Run” action. If the image has not been downloaded in current running instances, INSTANCE label will show as “null”. User can select the instance type they would like, customize the command line to run, and output like Amazon S3 bucket.

Once running docker image, user can find the launched tasks in Cloud Task list, each task display some details include image names, instance type, status, launched time, command, and instance id.