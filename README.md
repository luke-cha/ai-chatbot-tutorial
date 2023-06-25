# Creating an AI Chatbot Using Sendbird

In this tutorial, we're going to reveal the secrets behind creating a powerful AI chatbot using the Sendbird platform. AI chatbots, designed to provide top-tier responses to user inquiries, enhance the interaction experience by learning from previous chat records. But here's the exciting part - by leveraging Sendbird's AI Chatbot, you're not just creating a chatbot, you're creating your very own personalized AI assistant.
This system allows for seamless integration of knowledge-based chatbots into your channels. The best part? It's incredibly straightforward. Yes, you heard it right. With Sendbird, creating your AI chatbot isn't just possible, it's easy! Embrace the chance to transform the way you interact with your users, making their experience richer and more engaging. This is not just about creating a chatbot, it's about empowering your platform with the intelligence and responsiveness of AI. Step into the future, it's easier than you think!

## Prerequisites
- **Sendbird Account:** Go to [Sendbird Dashboard](https://dashboard.sendbird.com/) and create an account for a free trial. If you already have a Sendbird account, sign into your account.
- **Create a Application:**
  1. Create a new application by clicking **Create +** at the bottom right of your screen.
  2. Enter a name for your application. Choose a **Product Type** and **Region**. Then, click **Confirm**.
  3. Click the application you just created under **Applications**. You will see the application's Application ID which you will need when initializing the Chat SDK.
- **Knowledge Base Source:** Prepare data for AI ChatBot to reference in PDF or txt format. This data will serve as the Knowledge Base Source that AI Chatbot will use to generate responses.
  - Examples for Tutorial
    - PDF: [Italian CookBook Pdf file](https://drive.google.com/file/d/1uZmBBDEutwj5PAoXSJggZStj6ISwte5H/view)
    - URL: [Khan Academy](https://www.khanacademy.org/)

## 1. Navigate to Your Sendbird Application
1. Navigate to the application you created on the Sendbird Dashboard.
2. In the dashboard, navigate to the **Chat** menu and click on **AI Chatbot** under it.
   <img width="1000" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/e7d00cf0-fcf0-440b-8506-b46c077fff0d">

## 2. Set Up Your AI Chatbot
1. Click on the **Create Bot** button to set up a new AI chatbot.
2. In the **Bot Name** field, enter **Bot Name** you want, and make sure to select a unique **Bot ID**(will be used to invite Bot when creating a new Chat Room).
3. For the **Bot AI Engine**, select **OpenAI ChatGPT** for this time.
4. Specify the **Knowledge Base Source**. There are three options:
   - None: This uses the basic OpenAI Model, and you can adjust the specific parameters to suit your needs.
     <img width="300" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/c6912865-a88c-4e9f-b7cf-99569ffee8ae">

   - File: In this option, you can select a **PDF** or **txt** file as the Knowledge Base Source.
     <img width="600" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/7210bafe-1d42-4593-aae2-180cd6375689">

   - URL: In this option, the contents of a specified **URL** will be automatically analyzed and used as the Knowledge Base Source.
     <img width="600" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/356bd70d-9e47-4638-8687-1cd2f00abe56">

5. Click on the **Create** button to create your AI Chatbot.

## 3. Testing Your AI Chatbot
After your chatbot has been created, you can start testing conversations directly from the web interface.
<img width="800" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/f1d39df3-b50a-4c6d-a419-ef4bca5dcb87">

## 4. Next Step

Introducing the [Sendbird Chat AI Widget](https://github.com/sendbird/chat-ai-widget/), a tool I developed to make it even easier to use Sendbird Bots. By simply inputting your Sendbird App ID and Bot ID, you can quickly apply the Sendbird Chat AI Widget to enhance your AI Bot capabilities.

1. Create a `React Project`.
2. Install `ChatAIWidget` NPM Library.
3. Modify `App.js`.
4. Run it!

### 4.1. Customer Service Chat Support

The Sendbird Chat AI Widget is an excellent tool for customer service chat support. Utilize the AI Bot to implement automated responses and pre-register frequently asked questions. The AI Bot can handle real-time user inquiries and provide assistance with problem-solving.

 - Example: You can chat with the United States Consumer Financial Protection Bureau Support Bot
   
### 4.2. Shopping and Reservation Support

The Sendbird Chat AI Widget can be applied to support shopping websites and reservation platforms. With the AI Bot, you can promptly respond to queries regarding product information, stock availability, and reservation inquiries. Additionally, the AI Bot can offer personalized recommendations based on specific user demands, enhancing the overall user experience.

 - Example: You can chat with Airbnb Customer Service Bot
 
### 4.3. Learning Support

The Sendbird Chat AI Widget can also be leveraged for educational purposes. Use the AI Bot to answer students' questions, guide them through problem-solving processes, and provide information on learning materials and schedules. The AI Bot can interact with users to improve their learning experiences.

 - Example: You can chat with [Khan Academy Bot](https://sendbird.github.io/chat-ai-widget/)

In addition to these examples, the Sendbird Chat AI Widget can be utilized in various fields to develop AI Bot-powered services. For detailed information on the features and usage of the Sendbird Chat AI Widget, please refer to the GitHub repository at [https://github.com/sendbird/chat-ai-widget/](https://github.com/sendbird/chat-ai-widget/).

Please feel free to customize and format the content according to your requirements and the structure of your documentation.

### 4.3. Multi-Platform Support

Also another advantages of Sendbird is that it provides a variety of SDKs and UIKit. This makes it easy to integrate chat functionality directly into your platforms.

- Android([SDK](https://sendbird.com/docs/chat/v4/android/getting-started/send-first-message), [UIKit](https://sendbird.com/docs/uikit/v3/android/introduction/send-first-message))
- iOS([SDK](https://sendbird.com/docs/chat/v4/ios/getting-started/send-first-message), [UIKit](https://sendbird.com/docs/uikit/v3/ios/introduction/send-first-message))
- Javascript([SDK](https://sendbird.com/docs/chat/v4/javascript/getting-started/send-first-message))
- React([UIKit](https://sendbird.com/docs/uikit/v3/react/overview))
- React-Native([UIKit](https://sendbird.com/docs/uikit/v3/react-native/overview))
- Flutter([SDK](https://sendbird.com/docs/chat/v4/flutter/getting-started/send-first-message))
- Unity([SDK](https://sendbird.com/docs/chat/v3/unity/quickstart/send-first-message))
- Unreal([SDK](https://sendbird.com/docs/chat/v3/unreal/getting-started/send-first-message))
- .Net([SDK](https://sendbird.com/docs/chat/v3/dotnet/quickstart/send-first-message))


You can proceed with the process of creating AI Chatbot by referencing this tutorial. You can implement each step in detail and expand additional functions as needed. Best of luck with your project!
