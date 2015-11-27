# learninglocker-lrs-build
Build for a Learning Record Store based on Learninglocker

The LRS(Learning Record Store) learning locker has been deployed into the CSL VPC in AWS ;-) To access the site, just browse to [https://lrs.cstools.co.uk/]
Note; The site is only accessible from AviationHouse.

Workflow: 
* push to git@github.com:crossgovernmentservices/learninglocker-lrs-build.git
* circle should perform tests once we start defining them
* dockerhub gets the rebuild instruction from circle
* dockerhub instructs tutum to redeploy the service to aws

(please note that apart from the push to github.  Everything else happens programatically)

github -> circleCI -> DockerHub -> tutum -> AWS
