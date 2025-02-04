
# rasa init
# rasa inspect

nlu-20241128-112645-wintry-work.tar.gz 

## traning NLU model

rasa train nlu

# start a server with your NLU model
rasa run --enable-api -m models/nlu.tar.gz

rasa run --enable-api -m models/nlu-20250204-094201-frosty-candela.tar.gz

# request predictions
curl localhost:5005/model/parse -d '{"text":"hello"}'