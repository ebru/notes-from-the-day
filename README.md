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


### 13.1.21
**Resolve merge conflicts keeping our/their changes**

To resolve conflict for all files we can keep our current branch's changes with `Xours` or merging branch with `Xtheirs`

```
git merge -Xours
git merge -Xtheirs
```

For single file;

```
git checkout --ours src/components/index.js 
git checkout --theirs src/components/index.js 
```

---

### 30.1.21
**Install Chromium manually** if it is not automatically installed while installing Puppeteer

```
node node_modules/puppeteer/install.js
```

---

### 8.2.21
**Solving Problems with Technology** by University of Leeds & Institute of Coding

https://www.futurelearn.com/programs/solving-problems-with-technology

---

### 10.4.21
Loop over an array with a **delay between iterations**

```
const delayLoop = (fn, delay) => {
  return (name, i) => {
    setTimeout(() => {
      display(name);
    }, i * 1000);
  }
}

names.forEach(delayLoop(display, 1000))
```

https://travishorn.com/delaying-foreach-iterations-2ebd4b29ad30

---

### 13.7.21
**If you do one thing** this month...

https://www.theguardian.com/lifeandstyle/series/if-you-do-one-thing
