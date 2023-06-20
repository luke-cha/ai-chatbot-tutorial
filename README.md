# Creating an AI Chatbot Using Sendbird

In this tutorial, we will guide you on how to create an AI chatbot using the Sendbird platform. AI chatbots generate optimal responses to user inquiries and enhance the user experience by utilizing previous chat records. By using Sendbird's AI Chatbot, it is important to emphasize that you can easily create such sophisticated AI chatbots on various platforms. This allows you to effortlessly incorporate knowledge-based chatbots into your channels.

## Prerequisites
- **Sendbird Account:** Go to [Sendbird Dashboard](https://dashboard.sendbird.com/) and create an account for a free trial. If you already have a Sendbird account, sign into your account.
- **Create a Application:**
  1. Create a new application by clicking **Create +** at the bottom right of your screen.
  2. Enter a name for your application. Choose a **Product Type** and **Region**. Then, click **Confirm**.
  3. Click the application you just created under **Applications**. You will see the application's Application ID which you will need when initializing the Chat SDK.
- **Knowledge Base Source:** Prepare data for Clark to reference in PDF or txt format. This data will serve as the Knowledge Base Source that Clark will use to generate responses.
  - I will Prepare [Italian CookBook Pdf file](https://drive.google.com/file/d/1uZmBBDEutwj5PAoXSJggZStj6ISwte5H/view)
  - And Prepare [Korean Food Recipes](https://thewoksoflife.com/16-easy-korean-recipes/)

## 1. Navigate to Your Sendbird Application
1. Navigate to the application you created on the Sendbird Dashboard.
2. In the dashboard, navigate to the "Chat" menu and click on "AI Chatbot" under it.
   <img width="1000" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/e7d00cf0-fcf0-440b-8506-b46c077fff0d">

## 2. Set Up Your AI Chatbot
1. Click on the **Create Bot** button to set up a new AI chatbot.
2. In the **Bot Name** field, enter **Korea Food Master**, and make sure to select a unique **Bot ID**.
3. For the **Bot AI Engine**, select **OpenAI ChatGPT**. (Note: Google Bard is currently under development.)
4. Specify the **Knowledge Base Source**. There are three options:
   - None: This uses the basic OpenAI Model, and you can adjust the specific parameters to suit your needs.
     <img width="400" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/005398f0-130f-478f-9121-c1d9795378bb">

   - File: In this option, you can select a **PDF** or **txt** file as the Knowledge Base Source.    
     <img width="500" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/47d9410d-fce2-46c8-a118-b9cd2ffb12c3">


   - URL: In this option, the contents of a specified **URL** will be automatically analyzed and used as the Knowledge Base Source.
     <img width="500" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/235d367d-edf5-4cd7-b0ba-6b9a5329605c">



5. Click on the **Create** button to create your AI Chatbot.

## 3. Testing Your AI Chatbot
After your chatbot has been created, you can start testing conversations directly from the web interface.
<img width="800" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/6f52597a-fdf8-4be4-99ed-d2e57e7e102c">


## 4. Sendbird SDK and UIKit
One of the main advantages of Sendbird is that it provides a variety of SDKs and UIKit. This makes it easy to integrate chat functionality directly into your platforms.

- Android(Link: TBD)
   1. Set a application ID
     ```
     ~~~
     ```
   2. Make a Chatroob with AI Chatbot
     ```
     ~~~~
     ```  

   <img width="277" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/0239b765-441d-49c1-afec-803803384538">

- iOS(?)
- React(?)

## 5. Utilizing Chat History
You can utilize previous chat history to enhance the user experience AI Chatbot.

- (TBD)

You can proceed with the process of creating AI Chatbot by referencing this tutorial. You can implement each step in detail and expand additional functions as needed. Best of luck with your project!
