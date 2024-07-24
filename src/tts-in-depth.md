# TTS in Depth

**TTS Helper** can feel a bit overwhelming with all the settings it has and how they're spread out in the application.

Here's an overview of areas that can trigger TTS:

### Twitch connection
- **Random Message Chance**: You can change this input from 0 to 100, and every time a message from chat is sent, it'll "roll a chance" if that message counts as a TTS request.
- **Redeem**: Setup some Twitch redeems (that take text) to trigger TTS.
  - **Redeem**: This (poorly) named input will read whatever the user passes in as TTS.
  - **ChatGPT Redeem**: This redeem, when used, will forward user messages to your **configured** ChatGPT model.
    - This input doesn't show up if the ChatGPT page is disabled.
- **Bits**: If enabled, any messages with "cheers" will be read.
- **Followers**: If enabled, _your_ custom response will be read.
- **Subscriptions**: Normal and gift subs.
  - Both support different custom responses that will be read.
  - If enabled, you can read the users message, if one is included, before the custom response.

### Chat Settings
There are two chat commands that can be configured. **General** and **ChatGPT**.    
They're exactly the same when configuring.
- If enabled, users that use the specified **Command** can trigger TTS.
  - **User Permissions** is there to help you limit who can use these commands.
- **ChatGPT**: If enabled, users that use the **Command** will have their message forwarded to your customized **ChatGPT** model.
  - This will cause TTS to play as OpenAI generates a response for the above message.

### TTS Helper API
TTS Helper has an API third party apps can send request to, [see more here](./tts-api.md).  
If a request is made to TTS Helper via the API, it will trigger TTS.