# Creating an AI Chatbot Using Sendbird

In this tutorial, we guide you on how to create an AI chatbot named using the Sendbird platform. AI Chatbot generates optimal responses to user inquiries and improves the user experience by utilizing previous chat records.

## Prerequisites
- **Sendbird Account:** Create and sign in to your account on the Sendbird website.
- **Create a Application:** Create a new application on the Sendbird dashboard. You can specify the application name and other settings.
- **Knowledge Base Source:** Prepare data for Clark to reference in PDF or txt format. This data will serve as the Knowledge Base Source that Clark will use to generate responses.
  - I will Prepare [Italian CookBook Pdf file](https://drive.google.com/file/d/1uZmBBDEutwj5PAoXSJggZStj6ISwte5H/view)
  - And Prepare [Korean Food Recipes](https://thewoksoflife.com/16-easy-korean-recipes/)

## 1. Navigate to Your Sendbird Application
1. Navigate to the application you created on the Sendbird Dashboard.
2. In the dashboard, navigate to the "Chat" menu and click on "AI Chatbot" under it.
   ![image](https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/0cc6cafd-ba02-44e4-b710-3afacf4f9e44)

## 2. Set Up Your AI Chatbot
1. Click on the "Create Bot" button to set up a new AI chatbot.
2. In the "Bot Name" field, enter "Korea Food Master", and make sure to select a unique "Bot ID".
3. For the "Bot AI Engine", select "OpenAI ChatGPT". (Note: Google Bard is currently under development.)
4. Specify the Knowledge Base Source. There are three options:
   - None: This uses the basic OpenAI Model, and you can adjust the specific parameters to suit your needs.
     <img width="300" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/005398f0-130f-478f-9121-c1d9795378bb">

   - File: In this option, you can select a PDF or txt file as the Knowledge Base Source.    
     <img width="500" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/1051dae9-c7d4-4ac1-8dcb-759b0656bcf2">

   - URL: In this option, the contents of a specified URL will be automatically analyzed and used as the Knowledge Base Source.
     <img width="500" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/d7494b78-8eb8-4b19-988b-ff606b1d1855">


5. Click on the "Create" button to create your AI Chatbot.

## 3. Testing Your AI Chatbot
After your chatbot has been created, you can start testing conversations directly from the web interface.
<img width="800" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/6f52597a-fdf8-4be4-99ed-d2e57e7e102c">


## 4. Sendbird SDK and UIKit
One of the main advantages of Sendbird is that it provides a variety of SDKs and UIKit. This makes it easy to integrate chat functionality directly into your platforms.

- Android example ~~~ (TBD)

## 5. Utilizing Chat History
You can utilize previous chat history to enhance the user experience AI Chatbot.

- (TBD)

You can proceed with the process of creating AI Chatbot by referencing this tutorial. You can implement each step in detail and expand additional functions as needed. Best of luck with your project!
