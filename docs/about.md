# About GeoNEX

GEONEX is a web-based scientific platform for addressing on the key challenges of data-driven Geostationary (GEO) datasets, including but are not limited to, access to sufficient computing resources, massive data transfer, standardized analysis workflows and reproducibility to communicate analyses so that they can be reused and extended. Framework and user interface improvements now enable GEONEX to be used for streamlining analyzing tens of thousands of CONUS as well as Full Disk Scan of GOES16 and Himawari-9.



The new generation of GOES satellites carry the Advanced Baseline Imager (ABI) with spectral, spatial and radiometric resolutions comparable to EOS workhorse MODIS. More importantly ABI provides observations at 5-15 minute intervals offering exciting possibilities for producing robust biophysical variables by overcoming cloud cover, enabling studies of local-to-regional biosphere-atmosphere interactions, and operational decision-making in agriculture, forestry and range management.



The NASA Earth Exchange (NEX) team has been collaborating with the NOAA scientists and planning several GOES/ABI products for land surface monitoring. Many of the proposed products will leverage NASA’s investments in EOS algorithms. Started in 2017, GEONEX continues to focus on the key challenges of data-driven earth science, including but are not limited to, access to sufficient computing resources, massive data transfer, standardized analysis workflows and reproducibility to communicate analyses so that they can be reused and extended. During the last two years, the GEONEX team have made substantial improvements to the core framework, user interface, tools, and training materials. Framework and user interface improvements now enable GEONEX to be used for streamlining analyzing tens of thousands of CONUS as well as Full Disk Scan of GOES16/17 and Himawari-8 , and 7 standardized land products are now produced on GEONEX.



## GEONEX Concepts

- GEONEX Account - You need to create it to get access to GEONEX resources, including AWS EC2 instances, repos, containers, tasks and buckets.
- Buckets - AWS S3 buckets, used as input and output storage of GEONEX products
- Repos - a dockerized image, within it a combination of a file system and GEO application was built. It can be hosted on public docker registry services (hub.docker; AWS ECR; gcr.io)
- Containers - a standard unit on GEONEX approved by the administrator to finish specific processing/analysis jobs
- Runner - the runtime instance of a GEONEX containers (repo).
- Tasks  - containers related to specific output buckets, which can be browsed in the viewer



## Contact

Write to us (geonex84@gmail.com) to get an account on GEONEX.