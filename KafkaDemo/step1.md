#install Kafka
Folder for Producer and Consumer
`mkdir console-consumer-producer-basic && cd console-consumer-producer-basic`{{execute}}
##Get Confluent Platform



Now launch Confluent Platform by running:
`docker-compose up -d`{{execute}}

##Create a topic
Your first step is to create a topic to produce to and consume from. Use the following command to create the topic:
`docker-compose exec broker kafka-topics --create --topic example-topic --bootstrap-server broker:9092 --replication-factor 1 --partitions 1`{{execute}}

Start a console consumer
Next let’s open up a console consumer to read records sent to the topic you created in the previous step.

From the same terminal you used to create the topic above, run the following command to open a terminal on the broker container:
`docker-compose exec broker bash`{{execute}}

From within the terminal on the broker container, run this command to start a console consumer:
`kafka-console-consumer --topic example-topic --bootstrap-server broker:9092 `{{execute}}

## Testing

### Producer
`docker-compose exec broker bash'{{execute}}
Use the second terminal for executing following commnad
'kafka-console-producer --topic example-topic --broker-list broker:9092'{{execute HOST2}}


Try typing one line at a time, hit enter and go back to the console consumer window and look for the output. Or, you can select all the records and send at one time.
Example 
the
lazy
fox
jumped over the brown cow


At the end press CTRL +C 

### Consumer
