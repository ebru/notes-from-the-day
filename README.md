# notes from the day.
This is a little diary for me to track the progress, learning or any finding for each day.

I have taken some notes as little snippets starting in May 2019 that I have found useful to keep as a reminder or just with the purpose of setting starting points. 

Since I have really enjoyed reading them again some time to time, I decided to make this public considering it might be useful for anyone and keep it in this way from now on.

There might be things that I have expressed, known or typed wrong. If there is anything you would like to fix please feel free to open a pull request.

Here go the ones so far, happy learning 🚀
---

| [2020](https://github.com/ebru/notes-from-the-day/blob/master/2020.md) | [2019](https://github.com/ebru/notes-from-the-day/blob/master/2019.md) |
|--|--|
|  |  |


### 1.1.20
**Authentication vs Authorization**

Authentication is the process of ascertaining that somebody really is who they claim to be.

`Authentication = login + password (who you are)`

Authorization refers to rules that determine who is allowed to do what. E.g. Adam may be authorized to create and delete databases, while Usama is only authorised to read.

`Authorization = permissions (what you are allowed to do)`

In terms of web apps, authentication is when you check login credentials to see if you recognize a user as logged in, and authorization is when you look up in your access control whether you allow the user to view, edit, delete or create content.

https://stackoverflow.com/questions/6556522/authentication-versus-authorization

---

### 5.1.20
Learn the Newest and Easiest **React Native Stack** on Udemy

https://www.udemy.com/course/how-to-make-a-full-stack-react-native-app-with-easy-backend/

I really liked this course since it explains things to the point in such a short time to get an overall idea of the concept. Kudos to instructor 👏🏻

---

### 20.1.20
React Native **UI Kits**

- **React Native Elements** - https://react-native-elements.github.io/react-native-elements/docs/overview.html
- **React Native UI Kitten** - https://akveo.github.io/react-native-ui-kitten/docs/components/components-overview
- **NativeBase** - https://docs.nativebase.io/Components.html
- **Shoutem UI Kit** - https://shoutem.github.io/docs/ui-toolkit/components/typography


---

### 3.2.20
Advanced **JavaScript Concepts** on Udemy

https://www.udemy.com/course/advanced-javascript-concepts/

---

### 5.2.20
What is the difference between `while(true)` and `while(yield take(...))` in Redux-Saga?

- Don't need an action yielded from take effect, **while(yield take(...))**
- Otherwise, **while(true)**; const { limit, offset } = yield take...

https://github.com/redux-saga/redux-saga/issues/684

---

### 18.2.20
What is the difference between `splice` and `slice`?

**splice()** changes the original array whereas **slice()** doesn't.

```
array -> [1,2,3,4,5]
console.log(array.splice(2)); // [3,4,5]
```

The original array is affected resulting in array being [1, 2]

```
array -> [1,2,3,4,5]
console.log(array.slice(2)); // [3,4,5]
```
The original array is **NOT** affected with resulting in array being [1, 2, 3, 4, 5]

https://stackoverflow.com/questions/37601282/javascript-array-splice-vs-slice

---

### 23.2.20
- **How burnout makes us less creative** | The Way We Work, a TED series

https://www.youtube.com/watch?v=Dvhu2OK7ffg

- **Apollo GraphQL Tutorial** - Learn how to build full-stack apps with Apollo

https://www.apollographql.com/docs/tutorial/introduction/


---

### 1.3.20

```
"that even the ugliest of places can be beautiful, as long as you take the time to look.
that it's okay to get lost, as long as you find your way back."

— all the bright places
```

---

### 26.3.20

Yey! I wrote an article.

**a journey of making a little side project.**

https://medium.com/@ebrukye/a-journey-of-making-a-little-side-project-d18088271876

---

### 23.4.20

**Update versions of all packages in package.json to latest**

`yarn upgrade --latest`

---

### 2.5.20

- An easy way to apply **authentication flow with Netlify Identity** without a server need

Netlify Identity + https://github.com/netlify/gotrue-js

Demo site: https://gotruejs-playground.netlify.app/

- Deep learning **color generator** - Eva Design System

https://colors.eva.design/

---

### 1.7.20

Taking a break from 9-5. https://medium.com/@ebrukye/taking-a-break-from-9-5-1a08f9ac938f

A new journey begins with **Noe Crafts** 🎉 https://noecrafts.com

---

### 2.7.20

> "First and most important, the quest for personal freedom lies in the pursuit of value for others. Get this right from the beginning and the rest will be much easier. Always ask, `How can I help people more?`" 

— The $100 Startup by Chris Guillebeau

---

### 8.8.20
- Get **SSH public key**

```
ssh-keygen
cat ~/.ssh/id_rsa.pub
```

- Install **yarn** and **docker-compose** on Ubuntu

```
sudo apt remove cmdtest // special case
sudo apt remove yarn // special case
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt-get update  
sudo apt-get install yarn
```
```
sudo apt-get install docker-compose
```
