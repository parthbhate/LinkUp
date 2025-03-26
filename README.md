
## ⚡ Quick Setup

1. Sign up on [VideoSDK](https://app.videosdk.live/) to grab your API Key and Secret.
2. Familiarize yourself with [Token](https://docs.videosdk.live/javascript/guide/video-and-audio-calling-api-sdk/authentication-and-token)

## 🛠 Prerequisites

You must have the following installed:

- Node.js v12+
- NPM v6+ (comes pre-installed with newer Node versions)
- A valid [Video SDK Account](https://app.videosdk.live/signup)

## 📦 Running the Sample App

Follow these steps to get the sample app up and running:

### Step 1: Clone the Repository

```sh
git clone https://github.com/videosdk-live/videosdk-rtc-javascript-sdk-example.git
```

### Step 2: Set Up Environment Variables

Copy the example environment file:

```bash
cp config.example.js config.js
```

### Step 3: Configure Your `config.js` File

Generate a temporary token from your [**Video SDK Account**](https://app.videosdk.live/signup) and update the `config.js` file:

```
TOKEN="Your Token Here"
```

### Step 4: Run the app

```sh
npm install -g live-server
live-server --port=8000
```

## 🧠 Key Concepts

Understand the core components of our SDK:

- `Meeting` - A Meeting represents Real-time audio and video communication.

  **` Note: Don't confuse the terms Room and Meeting; both mean the same thing 😃`**

- `Sessions` - A particular duration you spend in a given meeting is referred as a session, you can have multiple sessions of a specific meetingId.
- `Participant` - A participant refers to anyone attending the meeting session. The `local participant` represents yourself (You), while all other attendees are considered `remote participants`.
- `Stream` - A stream refers to video or audio media content that is published by either the `local participant` or `remote participants`.


## 🔐 Token Generation

The token is used to create and validate a meeting using API and also initialize a meeting.

🛠️ `Development Environment`:

- You can use a temporary token for development. To create one, go to the VideoSDK's [dashboard](https://app.videosdk.live/api-keys) .

🌐 `Production Environment`:

- You must set up an authentication server to authorize users for production. To set up an authentication server, please take a look at our official example repositories. [videosdk-rtc-api-server-examples](https://github.com/videosdk-live/videosdk-rtc-api-server-examples)
