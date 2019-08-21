
# Sysmon server
## Install required dependencies
| Download Page| Notes |
|:-:|-|
| [Golang](https://golang.org/dl/)| Install Go version that support modules feature (>= Go 1.13)|
| [Nodejs](https://nodejs.org/en/download/)| Install latest LTS Version|
| [PostgreSQL](https://www.postgresql.org/download/)|After installed: </br> <li><code>sudo -u postgres createuser --createdb --pwprompt gosysmon</code> </br> Enter your password for user gosysmon. You also need to set your password in gosysmon/config.yml</li><li><code>createdb --host=localhost --username=gosysmon --password gosysmon</code></li><li><code>psql --host=localhost --username=gosysmon --password gosysmon -f resources/gosysmon.sql</code></li>|
| [Redis](https://redis.io/download)| Although it is designed to be accessed by trusted clients inside trusted environments. It is still recommended to provide an authentication layer to it. </br>We are going to set the password the the “default” user</br>Open redis.conf and looking for the line “**# requirepass foobared**”. Uncomment and set your password like this:</br>**requirepass gosysmon** |
| [Kafka](https://kafka.apache.org/downloads)| You need to create a topic named gosysmon:</br><code>bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic winsysmon</code></br>To verify the created topic:</br><code>bin/kafka-topics.sh --list --bootstrap-server localhost:9092|</code> 
## Start the monitor system: 
1. Pull project code from github repository.
2. Manage gosysmon service options:
   
<pre>
	<code>
	-i				:install service
	-u				:uninstall service
	-c config_file.xml		:update gosysmon service configuration
	</code>
</pre>

3. To compile and run project:
   
<code> make && ./gosysmon</code>
   

   
	

# Sysmon server
## Install required dependencies
| Download Page| Notes |
|:-:|-|
| [Golang](https://golang.org/dl/)| Install Go version that support modules feature (>= Go 1.13)|
| [Nodejs](https://nodejs.org/en/download/)| Install latest LTS Version|
| [PostgreSQL](https://www.postgresql.org/download/)|After installed: </br> <li><code>sudo -u postgres createuser --createdb --pwprompt gosysmon</code> </br> Enter your password for user gosysmon. You also need to set your password in gosysmon/config.yml</li><li><code>createdb --host=localhost --username=gosysmon --password gosysmon</code></li><li><code>psql --host=localhost --username=gosysmon --password gosysmon -f resources/gosysmon.sql</code></li>|
| [Redis](https://redis.io/download)| Although it is designed to be accessed by trusted clients inside trusted environments. It is still recommended to provide an authentication layer to it. </br>We are going to set the password the the “default” user</br>Open redis.conf and looking for the line “**# requirepass foobared**”. Uncomment and set your password like this:</br>**requirepass gosysmon** |
| [Kafka](https://kafka.apache.org/downloads)| You need to create a topic named gosysmon:</br><code>bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic winsysmon</code></br>To verify the created topic:</br><code>bin/kafka-topics.sh --list --bootstrap-server localhost:9092|</code> 
## Start the monitor system: 
1. Pull project code from github repository.
2. Manage gosysmon service options:
   
<pre>
	<code>
	-i				:install service
	-u				:uninstall service
	-c config_file.xml		:update gosysmon service configuration
	</code>
</pre>

3. To compile and run project:
   
<code> make && ./gosysmon</code>
   

   
	

# Sysmon server
## Install required dependencies
| Download Page| Notes |
|:-:|-|
| [Golang](https://golang.org/dl/)| Install Go version that support modules feature (>= Go 1.13)|
| [Nodejs](https://nodejs.org/en/download/)| Install latest LTS Version|
| [PostgreSQL](https://www.postgresql.org/download/)|After installed: </br> <li><code>sudo -u postgres createuser --createdb --pwprompt gosysmon</code> </br> Enter your password for user gosysmon. You also need to set your password in gosysmon/config.yml</li><li><code>createdb --host=localhost --username=gosysmon --password gosysmon</code></li><li><code>psql --host=localhost --username=gosysmon --password gosysmon -f resources/gosysmon.sql</code></li>|
| [Redis](https://redis.io/download)| Although it is designed to be accessed by trusted clients inside trusted environments. It is still recommended to provide an authentication layer to it. </br>We are going to set the password the the “default” user</br>Open redis.conf and looking for the line “**# requirepass foobared**”. Uncomment and set your password like this:</br>**requirepass gosysmon** |
| [Kafka](https://kafka.apache.org/downloads)| You need to create a topic named gosysmon:</br><code>bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic winsysmon</code></br>To verify the created topic:</br><code>bin/kafka-topics.sh --list --bootstrap-server localhost:9092|</code> 
## Start the monitor system: 
1. Pull project code from github repository.
2. Manage gosysmon service options:
   
<pre>
	<code>
	-i				:install service
	-u				:uninstall service
	-c config_file.xml		:update gosysmon service configuration
	</code>
</pre>

3. To compile and run project:
   
<code> make && ./gosysmon</code>
   

   
	

# Sysmon server
## Install required dependencies
| Download Page| Notes |
|:-:|-|
| [Golang](https://golang.org/dl/)| Install Go version that support modules feature (>= Go 1.13)|
| [Nodejs](https://nodejs.org/en/download/)| Install latest LTS Version|
| [PostgreSQL](https://www.postgresql.org/download/)|After installed: </br> <li><code>sudo -u postgres createuser --createdb --pwprompt gosysmon</code> </br> Enter your password for user gosysmon. You also need to set your password in gosysmon/config.yml</li><li><code>createdb --host=localhost --username=gosysmon --password gosysmon</code></li><li><code>psql --host=localhost --username=gosysmon --password gosysmon -f resources/gosysmon.sql</code></li>|
| [Redis](https://redis.io/download)| Although it is designed to be accessed by trusted clients inside trusted environments. It is still recommended to provide an authentication layer to it. </br>We are going to set the password the the “default” user</br>Open redis.conf and looking for the line “**# requirepass foobared**”. Uncomment and set your password like this:</br>**requirepass gosysmon** |
| [Kafka](https://kafka.apache.org/downloads)| You need to create a topic named gosysmon:</br><code>bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic winsysmon</code></br>To verify the created topic:</br><code>bin/kafka-topics.sh --list --bootstrap-server localhost:9092|</code> 
## Start the monitor system: 
1. Pull project code from github repository.
2. Manage gosysmon service options:
   
<pre>
	<code>
	-i				:install service
	-u				:uninstall service
	-c config_file.xml		:update gosysmon service configuration
	</code>
</pre>

3. To compile and run project:
   
<code> make && ./gosysmon</code>
   

   
	

# Sysmon server
## Install required dependencies
| Download Page| Notes |
|:-:|-|
| [Golang](https://golang.org/dl/)| Install Go version that support modules feature (>= Go 1.13)|
| [Nodejs](https://nodejs.org/en/download/)| Install latest LTS Version|
| [PostgreSQL](https://www.postgresql.org/download/)|After installed: </br> <li><code>sudo -u postgres createuser --createdb --pwprompt gosysmon</code> </br> Enter your password for user gosysmon. You also need to set your password in gosysmon/config.yml</li><li><code>createdb --host=localhost --username=gosysmon --password gosysmon</code></li><li><code>psql --host=localhost --username=gosysmon --password gosysmon -f resources/gosysmon.sql</code></li>|
| [Redis](https://redis.io/download)| Although it is designed to be accessed by trusted clients inside trusted environments. It is still recommended to provide an authentication layer to it. </br>We are going to set the password the the “default” user</br>Open redis.conf and looking for the line “**# requirepass foobared**”. Uncomment and set your password like this:</br>**requirepass gosysmon** |
| [Kafka](https://kafka.apache.org/downloads)| You need to create a topic named gosysmon:</br><code>bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic winsysmon</code></br>To verify the created topic:</br><code>bin/kafka-topics.sh --list --bootstrap-server localhost:9092|</code> 
## Start the monitor system: 
1. Pull project code from github repository.
2. Manage gosysmon service options:
   
<pre>
	<code>
	-i				:install service
	-u				:uninstall service
	-c config_file.xml		:update gosysmon service configuration
	</code>
</pre>

3. To compile and run project:
   
<code> make && ./gosysmon</code>
   

   
	

# Sysmon server
## Install required dependencies
| Download Page| Notes |
|:-:|-|
| [Golang](https://golang.org/dl/)| Install Go version that support modules feature (>= Go 1.13)|
| [Nodejs](https://nodejs.org/en/download/)| Install latest LTS Version|
| [PostgreSQL](https://www.postgresql.org/download/)|After installed: </br> <li><code>sudo -u postgres createuser --createdb --pwprompt gosysmon</code> </br> Enter your password for user gosysmon. You also need to set your password in gosysmon/config.yml</li><li><code>createdb --host=localhost --username=gosysmon --password gosysmon</code></li><li><code>psql --host=localhost --username=gosysmon --password gosysmon -f resources/gosysmon.sql</code></li>|
| [Redis](https://redis.io/download)| Although it is designed to be accessed by trusted clients inside trusted environments. It is still recommended to provide an authentication layer to it. </br>We are going to set the password the the “default” user</br>Open redis.conf and looking for the line “**# requirepass foobared**”. Uncomment and set your password like this:</br>**requirepass gosysmon** |
| [Kafka](https://kafka.apache.org/downloads)| You need to create a topic named gosysmon:</br><code>bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic winsysmon</code></br>To verify the created topic:</br><code>bin/kafka-topics.sh --list --bootstrap-server localhost:9092|</code> 
## Start the monitor system: 
1. Pull project code from github repository.
2. Manage gosysmon service options:
   
<pre>
	<code>
	-i				:install service
	-u				:uninstall service
	-c config_file.xml		:update gosysmon service configuration
	</code>
</pre>

3. To compile and run project:
   
<code> make && ./gosysmon</code>
   

   
	
