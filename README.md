# Create an AI Chatbot with Sendbird

This tutorial demonstartes how to create a powerful AI chatbot using the Sendbird platform.

AI chatbots are designed to provide comprehensive responses to user inquiries by learning from previous chat records, thus enhancing user experience. By leveraging Sendbird's AI chatbot, it can go beyond a simple chatbot to a personalized AI assistant with a seamless, easy-to-follow integration of knowledge-based chatbots into channels. You also can add or customize additional functions as needed after implementing the following codes. These AI chatbots can empower your service with a richer and more engaging user experience with a personalized assistance. 

<img width="800" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/a61a4b2e-730a-4f3f-b326-11eadb61a55b">

## Prerequisites

- **Sendbird account:**
  1. Go to [Sendbird Dashboard](https://dashboard.sendbird.com/) and create an account for a free trial. If you already have a Sendbird account, sign into your account.
  
- **Application ID:**
  1. Create a new Sendbird application by clicking **Create +** at the bottom-right corner of your screen.
  2. Enter a name for your application. Choose a **Product Type** and **Region**. Then, click **Confirm**.
  3. Click the application you just created under **Applications** on the top-left corner of your screen. 
  4. On the **Overview** page, you can find the **Application ID** which you will need when initializing the Chat SDK.
  
- **Knowledge Base Source:** Prepare data source in `PDF` or `txt` format or its `URL` so that AI chatbot can learn in advance. This data will serve as the Knowledge Base Source that AI chatbot will use to generate responses.
  - References for tutorial
    - PDF: [Italian CookBook Pdf file](https://drive.google.com/file/d/1uZmBBDEutwj5PAoXSJggZStj6ISwte5H/view)
    - URL: [Khan Academy](https://www.khanacademy.org/)

## Integration

### Step 1: Navigate to your Sendbird Application
1. Go to the application you created on Sendbird Dashboard.
2. In the left menu bar on the dashbaord, click **AI chatbots** under **Chat**.
   <img width="1000" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/e7d00cf0-fcf0-440b-8506-b46c077fff0d">

### Step 3: Set up your AI chatbot
1. Click on the **Create bot +** button to set up a new AI chatbot.
2. In the **Bot Name** field, enter a unique **Bot Name** and **Bot ID** of your choice. Store the ID becuase it's needed when creating a channel for the Bot.
3. For the **Bot AI engine**, select **OpenAI ChatGPT** for this time.
4. Specify **Knowledge Base Source**. There are three options:
   - None: the bot uses the basic OpenAI Model and you can adjust the specific parameters to your needs.
     
     <img width="300" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/c6912865-a88c-4e9f-b7cf-99569ffee8ae">

   - File: you can select a **PDF** or **txt** file. Supported formats are `.json`, `.txt`, `.md`, and `.pdf`. The maximum file size is 5MB.

     <img width="600" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/7210bafe-1d42-4593-aae2-180cd6375689">

   - URL: the contents of a specified **URL**(Maximum: 10 URLs (up to 1,000 URL subpages per URL)) will be automatically analyzed and used as the bot's Knowledge Base Source.
     
     <img width="600" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/356bd70d-9e47-4638-8687-1cd2f00abe56">

5. Click **Create**.

### Step 3: Testing your AI chatbot

After your chatbot is created, you can start a test conversation directly from the web interface.
<img width="800" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/f1d39df3-b50a-4c6d-a419-ef4bca5dcb87">

## Sendbird Chat AI Widget

Try [Sendbird Chat AI Widget](https://github.com/sendbird/chat-ai-widget/) for an easier implementation of Sendbird AI chatbots. Enter your Sendbird App ID and Bot ID - you can quickly apply Sendbird Chat AI Widget to enhance your AI chatbots capabilities.

1. Create `React Project`.
   
   ```bash
   npx create-react-app react-sample
   cd react-sample
   ```
   
2. Install `ChatAIWidget` NPM Library.

   ```bash
   npm install @sendbird/chat-ai-widget
   ```
   
3. Modify `src/App.js` as follows.

   ```jsx
   import logo from './logo.svg';
   import './App.css';
   import ChatAiWidget from "@sendbird/chat-ai-widget";
   
   function App() {
     return (
       <div className="App">
         <header className="App-header">
           <img src={logo} className="App-logo" alt="logo" />
           <p>
             Edit <code>src/App.js</code> and save to reload.
           </p>
           <a
             className="App-link"
             href="https://reactjs.org"
             target="_blank"
             rel="noopener noreferrer"
           >
             Learn React
           </a>
         </header>
         <ChatAiWidget
             applicationId="AE8F7EEA-4555-4F86-AD8B-5E0BD86BFE67"
             botId="khan-academy-bot"
         />
       </div>
     );
   }
    
   export default App;
   ```
   
4. Run the codes.

   ```bash
   npm start
   ```
   
 5. Then you will see the following web screen. Click **Widget** at the bottom-right corner.
   <img width="523" alt="image" src="https://github.com/sf-luke-cha/ai-chatbot-tutorial/assets/104121286/57494068-24d8-4ce3-83a1-243a866b0680">

## Use cases

### Education

Sendbird Chat AI Widget can also be leveraged for educational purposes. Use the AI chatbots to answer students' questions, guide them through problem-solving processes, and provide information on learning materials and schedules. The AI chatbots can interact with users to improve their learning experiences.

 - Example
   - You can chat with [Khan Academy Bot](https://sendbird.github.io/chat-ai-widget/)
   - [Sendbird Docs Bot](https://sendbird.com/docs)

### Customer service

Sendbird Chat AI Widget is an excellent tool for customer service chat support. Utilize AI chatbots to implement automated assistance to pre-registered frequently asked questions. The AI chatbots can handle user inquiries real-time.
  
### Shopping and reservation 

Sendbird Chat AI Widget can be applied to shopping and reservation platforms. With the AI chatbots, you can promptly respond to queries regarding product information, inventory status, and reservations. Additionally, the AI chatbots can offer personalized recommendations based on a user's specific demands, enhancing the overall user experience.

In addition to these examples, Sendbird Chat AI Widget can be utilized in various fields to develop AI chatbots-powered services. For detailed information on the features and usage of Sendbird Chat AI Widget, see our [GitHub repository for the widget](https://github.com/sendbird/chat-ai-widget/).

## Multi-platform support

Sendbird also provides SDKs and UIKit for a wide range of platforms, making it easier to integrate chat functionalities directly into your application.

- Android([SDK](https://sendbird.com/docs/chat/v4/android/getting-started/send-first-message), [UIKit](https://sendbird.com/docs/uikit/v3/android/introduction/send-first-message))
- iOS([SDK](https://sendbird.com/docs/chat/v4/ios/getting-started/send-first-message), [UIKit](https://sendbird.com/docs/uikit/v3/ios/introduction/send-first-message))
- Javascript([SDK](https://sendbird.com/docs/chat/v4/javascript/getting-started/send-first-message))
- React([UIKit](https://sendbird.com/docs/uikit/v3/react/overview))
- React-Native([UIKit](https://sendbird.com/docs/uikit/v3/react-native/overview))
- Flutter([SDK](https://sendbird.com/docs/chat/v4/flutter/getting-started/send-first-message))
- Unity([SDK](https://sendbird.com/docs/chat/v3/unity/quickstart/send-first-message))
- Unreal([SDK](https://sendbird.com/docs/chat/v3/unreal/getting-started/send-first-message))
- .Net([SDK](https://sendbird.com/docs/chat/v3/dotnet/quickstart/send-first-message))

