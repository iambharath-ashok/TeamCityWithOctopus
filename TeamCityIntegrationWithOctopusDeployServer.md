#	Octopus Deployment From TeamCity

##	Install Octopus on Windows Server 

- 	Download Octopus and run MSI

-------------------------------------------------------------------------------------------


##	Build Maven Application with TeamCity

-	Create Project and Repo URL
-	Give username and password
-	Create Build Steps WRT project
-	Create Build Steps to deploy to Octopus Deploy Server
-	Provide API Keys and artifact path 
-	Once build is completed successfully it will be pushed to Octopus deploy server


-----------------------------------------------------------------------------------------------------

##	TeamCity Integration With Octopus Deploy Server

-	Download and Install TeamCity
-	Install both Agent and Server Components as Windows Service
-	Create project and set all the configuration parameters, environment variables etc
-	Install Octopus Deployment server 
-	Install Octopus Deployment Plug-in into TeamCity 
-	Enable Octopus Plug-in
-	Create a dummy project and configure Octopus Deployment plug-in to copy artifact from TeamCity to Octopus Deployment Server
-	Provide VCS URL in TeamCity and add "Build Steps"
-	In "Build Step" provide details for Octopus packaging and publishing
-	Artifact will deployed from TeamCity to Octopus Deploy Server


-----------------------------------------------------------------------------------------------------

##	Deploying on IIS(Internet Information Service) Server with Octopus Deploy Server

- 	Create Infrastructure or Environment
-	Add IIS Server or Machine with any of the flavors i.e windows, linux, mac, azure, kubernetes

###	Install Tentacle agent on Remote Machine or Target Machine
-	Listening Tentacle
-	Polling Tentacle
-	Enable the port for Listening
-	Add Octopus Thumbprint
	
###	Add Tentacle Agent on Octopus Deploy Server

-	Add hostname and port
-	Add display name
-	Choose environments
- 	Add Roles
-	Add Tentacle Thumbprint on Octopus
-	Check the Health

###	Deploying Artifact From Octopus Deploy Server to IIS Server

-	Create a Project
-	Add Step to perform the activity of deployment to remote IIS server
-	Choose Step template
-	Give Step Name, Execution Location, Target Roles, Package Id
-	Configure Deployment Server 
	- 	Deployment server name
	-	Deployment Environment i.e java, .net, etc
	-	Port and other things
	
### Add Variable, Triggers, Channels, Release 

-	Variables are used to set the environment variables
-	Triggers are used to set up "How we want to deploy to server"
	-	Manual or Automatic
-	Channel is used to create the life cycle 
-	Release are used to select and set the release version
-	Click on Deploy to environment and Deploy

## https://octopus.com/docs/packaging-applications/build-servers/teamcity

















