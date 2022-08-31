# nhgis-assets

## Description
nginx image to serve content from `/pkg/ipums/istads/assets.nhgis.org/htdocs` at assets.nhgis.org. 


The `/crosswalks` and `/environmental` paths are served through the spatial web app due to those files requiring password protection, so this app redirects those paths to data2.nhgis.org.


## Deployment
Deployed using jenkins pipeline library. All pushes to master branch are deployed. Jenkins configuration at https://jenkins-master.pop.umn.edu/job/nhgis-assets/