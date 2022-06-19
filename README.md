# notes from the day.
This is a little diary for me to track the progress, learning or any finding for each day.

I have taken some notes as little snippets starting in May 2019 that I have found useful to keep as a reminder or just with the purpose of setting starting points. 

Since I have really enjoyed reading them again some time to time, I decided to make this public considering it might be useful for anyone and keep it in this way from now on.

There might be things that I have expressed, known or typed wrong. If there is anything you would like to fix please feel free to open a pull request.

Here go the ones so far, happy learning 🚀
---

| [2021](https://github.com/ebru/notes-from-the-day/blob/master/2021.md) | [2020](https://github.com/ebru/notes-from-the-day/blob/master/2020.md) | [2019](https://github.com/ebru/notes-from-the-day/blob/master/2019.md) |
|--|--|--|
|  |  |  |


### 3.1.22
- **Kurşun Geçirmez React Native Uygulamaları Oluşturmak - I**

https://faruko.space/building-bulletproof-react-native-applications

- **The Business of Building Apps**

https://youtu.be/poLzjLt2yqU

---

### 6.2.22
- New **VSCode** theme: ƒ - Darcula - Operator Mono/Italic

https://www.vscolors.com/themes/33474ff6-baf7-461f-8275-a44cfd27d13a-92e5d4da

---

### 10.3.22
- **React Query** in 100 Seconds

https://youtu.be/novnyCaa7To

- Fetching Data the Right Way

https://telerik.com/blogs/react-query-fetching-data-right-way

- Practical **React Query**

https://tkdodo.eu/blog/practical-react-query

Not everything should be handled by `react-query` or `redux` for example, like in the days it was a popular choice for each need. 
Especially wrapping all backend calls to a global state is meaningless.

Be aware of the needs of a global state and store; 

- For handling `backend state and its side effects` like `loading, error, data` -> `react-query`, `swr` etc.

- `Local global state` needs like token, theme, selectedLanguage etc. -> `context`, `zustand`, `redux` etc.

- Persistent storage -> AsyncStorage, encrpypted storages etc.


```
"For years, we've made the mistake of treating every state equally by treating our server data like client state.
We've finally realized that this is sub-optimal, because they have different needs.
Let's not make the same mistake again in the other direction by wanting to do everything with react query please."
- TkDodo
```

https://github.com/tannerlinsley/react-query/discussions/489

---

### 11.3.22
**Local and Push Notifications** in React Native

- Firebase: https://betterprogramming.pub/how-to-set-up-firebase-push-notifications-in-a-react-native-app-a9405af32093

- React Native Notifications: https://github.com/wix/react-native-notifications

- Notifee: https://notifee.app/react-native/docs/overview

- OneSignal: https://documentation.onesignal.com/docs/react-native-sdk-setup

- Expo Notifications: https://docs.expo.dev/versions/latest/sdk/notifications/

---

### 12.3.22

**Microinteractions & Animations** in React Native: Help users understand the UI by Catalin Miron

https://youtu.be/a5SgLyfiDnU

---

### 19.6.22

Cleaner data fetching with **react-query**

https://dev.to/siddharthvenkatesh/cleaner-data-fetching-with-react-query-4klg
