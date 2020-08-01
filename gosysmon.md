
# Sysmon server
## Install required dependencies
|| Download Page| Notes |
|-|-|-|
| Golang | https://golang.org/dl/ | Install Go version that support modules feature (>= Go 1.13)|
| Nodejs | https://nodejs.org/en/download/| Install latest LTS Version|
| PostgreSQL | https://www.postgresql.org/download/ | After installed: <br /> <li>sudo -u postgres createuser --createdb --pwprompt gosysmon<br />Enter your password for user gosysmon. You also need to set your password in gosysmon/config.yml</li><li>createdb --host=localhost --username=gosysmon --password gosysmon</li><li>psql --host=localhost --username=gosysmon --password gosysmon -f resources/gosysmon.sql</li> |
| Redis| https://redis.io/download| Although it is designed to be accessed by trusted clients inside trusted environments. It is still recommended to provide an authentication layer to it. </br>We are going to set the password the the “default” user</br>Open redis.conf and looking for the line “# requirepass foobared”. Uncomment and set your password like this:</br>**requirepass gosysmon** |
| Kafka| https://kafka.apache.org/downloads | You need to create a topic named gosysmon:</br> bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic winsysmon</br>To verify the created topic:</br>bin/kafka-topics.sh --list --bootstrap-server localhost:9092|
## Pull project code from github repository: 
	https://github.com/tiencong283/gosysmon
## Start the monitor system: 
1. Install gosysmon service:</br>
**./gosysmon -i** 
2. Uninstall all gosysmon service:</br>
**./gosysmon -u**
3. Update configuration of gosysmon service: 
./gosysmon -c config.xml
4. You need to compile project:</br>
    * Access to project folder gosysmon and run this command: make
    * Go to client folder, run this command: npm install && npm run build
	* run ./gosysmon in the project folder to start the dashboard, then open your web browser for starting monitor.
	
