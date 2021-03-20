Rasa Core Chatbot

Install Rasa core and create simple chatbot in windows

Install python3 latest version

Install Rasa core

Create a virtual environment virtualenv venv Successfully created the virtual environment

Activate the virtual environment .\venv\Scripts\activate

Install Rasa core pip install rasa

rasa installed successfully

Create project i. rasa init

 successfully created the project and running
Customize the chatbot

nlu.md
stories.md
domain.yml
we need change these 3 files

nlu.md what is intent? train data or keywords we need add in this files

domain.yml now we need to set response values

create templates and add in actions also we need to add the intent

stories.md now we need to make stories based on the intent and response

##intent name

action name
train rasa rasa train - successfully trained

run project rasa shell

now ask the intent questions

successfully running as we specified in the nlu and stories

Create Custom actions

create intent -> add in domain.yml
create custom actions in actions.py and add in domain.yml file
make stories in stories.md file
rasa train
open new cmd prompt and run actions rasa run actions
run rasa core & add the endpoints rasa shell --endpoints endpoints.yml
successfully created custom action

Custom UI for rasa chatbot

i have created the custom UI and added in the chatbot folder

index.html-> chat ui added

script.js -> using for ajax call to python chatbot

Lets view the ajax call

start the chatbot in cmd prompt

rasa run -m models --enable-api --cors "*" --debug

successfully added the UI in chatbot
