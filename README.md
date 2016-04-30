# RealTimeStorm

###Navigate to project home path
mvn clean package

### install redis as socket
on mac->  
brew install redis
redis-server
on cent os- > sudo service redis start
reference: http://jasdeep.ca/2012/05/installing-redis-on-mac-os-x/

###launch website
cd viz <br />
python app.py <br />

type http://127.0.0.1:5000/index

###trigger storm process
storm jar target/realtime-0.1-jar-with-dependencies.jar storm.TopNTweetTopology
