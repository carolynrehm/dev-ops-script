# setup
* create an ec2.  
* update the ec2 with `sudo yum update -y`  
* install git with `sudo yum install git -y`  
* use git to clone this repo with the script to install the rest of the software `git clone https://github.com/btkruppa/dev-ops-script.git`  
* navigate to the repo directory `cd dev-ops-script`
* run the script to install required software on the ec2, navigate into the repo and run `sh installv2.sh`
* it will make you select the version for java and javac
* after it runs if you want to do mvn commands exit and re-enter the ec2. If someone can get this better that would be great.
# jenkins
* jenkins should now be running on port 8080 of the ec2 with no addition to the url after the port
* to get the password run `sudo cat /var/lib/jenkins/secrets/initialAdminPassword` or if the path on jenkins says differently use the path it specifies
# tomcat
* there will be a separate tomcat on port 8090 that you can deploy wars to
