# Firebase Notification Project

This project demonstrates how to integrate Firebase Cloud Messaging (FCM) for push notifications in a web application using Firebase and jQuery.

## Features

- Retrieve and display the device token for push notifications.
- Receive and display notification data when the app is open and focused.
- Subscribe and unsubscribe from topics to manage notifications.
- Display notifications as toasts using Toastr library.
- Handle errors and provide user-friendly messages.

## Prerequisites

Before using this project, ensure you have the following prerequisites:

- Firebase Project: Create a Firebase project on the [Firebase Console](https://console.firebase.google.com/). Obtain the Firebase configuration object with your API keys.
- Firebase Cloud Messaging: Enable Firebase Cloud Messaging for your project.

## Installation

1. Clone this repository to your local machine:

```
git clone https://github.com/your-username/firebase-notification-project.git
```

2. Open the `index.html` file in your text editor or IDE.

3. Update the Firebase configuration with your own API keys in index.html and firebase-messaging-sw.js:

```
const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_AUTH_DOMAIN",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_STORAGE_BUCKET",
    messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
    appId: "YOUR_APP_ID",
    measurementId: "YOUR_MEASUREMENT_ID"
};
```

4. Update the cloudMessagingApiServerKey key:

```
    const cloudMessagingApiServerKey = 'CLOUD_MESSAGING_API_SERVER_KEY';
```

5. Update the VAPID key:

```
    const vapidKey = 'YOUR_VAPID_KEY';
```

6. To run the application, open the index.html file using ngrok. Ngrok allows you to expose your local server over the internet, ensuring Firebase Messaging works correctly.

## Usage

1. When you open the application, you will see your device token displayed.

2. Notification data will be displayed in the "Notification data will be received here" section when the app is open and focused.

3. To subscribe or unsubscribe from topics, enter the topic name and click the "Subscribe" or "Unsubscribe" button, respectively.

4. Toast notifications will be displayed to indicate success or error messages for subscription and unsubscription actions.

## License

This project is licensed under the MIT License.
