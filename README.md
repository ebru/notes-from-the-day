# notes from the day.
This is a little diary for me to track the progress, learning or any finding for each day.

I have taken some notes as little snippets starting in May this year that I have found useful to keep as a reminder or just with the purpose of setting starting points. 

Since I have really enjoyed reading them again some time to time, I decided to make this public considering it might be useful for anyone and keep it in this way from now on.

There might be things that I have expressed, known or typed wrong. If there is anything you would like to fix please feel free to open a pull request.

Here go the ones so far, happy learning 🚀

### 25.5.19
- Created a learning roadmap for full-stack web development.

`JavaScript ES6` `React` `Redux` `Node.js` `Express` `GraphQL` `Apollo` `MongoDB` `Mongoose` `AWS` `Docker`

- **CS50**'s Introduction to Computer Science by Harvard University on edX, **Week 0**

https://cs50.edx.org

- TED Talk: **Mitch Resnick: Let's teach kids to code**

https://www.youtube.com/watch?v=Ok6LbV6bqaE

- **DRY** - Do not repeat yourself!

---

### 26.5.19
- **(Right to Left (** The Mirror World

https://labs.spotify.com/2019/04/15/right-to-left-the-mirror-world/

- Building **Spotify’s New Web Player**

https://labs.spotify.com/2019/03/25/building-spotifys-new-web-player/

---

### 29.5.19
**Optimising SVGs** for Web Use

Part 1: https://medium.com/larsenwork-andreas-larsen/optimising-svgs-for-web-use-part-1-67e8f2d4035

Part 2: https://medium.com/larsenwork-andreas-larsen/optimising-svgs-for-web-use-part-2-6711cc15df46

Part 2½: https://medium.com/larsenwork-andreas-larsen/optimising-svgs-for-web-use-part-2-1-598815d74f9c

---

### 31.5.19
- Advanced Git Commands: **Rewriting History**

https://dzone.com/articles/advanced-git-commands-rewriting-history

```
git log --oneline // show git commit history in one line

git commit --amend --no-edit // add staged changes to the previous commit

git checkout master
git pull
git checkout feature/my-feature-branch
git rebase master // add the commits to the most up-to-date version of the master branch
git checkout master
git merge feature/my-feature-branch

git rebase -i master // interactive rebase, change the way git applies your commits

```

- **CS50**'s Introduction to Computer Science by Harvard University on edX, **Week 1**

---

### 5.6.19
- What **The Flexbox?!** (20 chapters)

https://flexbox.io/

- A Complete Guide to **Flexbox**

https://css-tricks.com/snippets/css/a-guide-to-flexbox/

---

### 12.6.19
New style! Oh My Zsh + Theme – **Bira** + iTerm Color Preset – **ayu**

https://ohmyz.sh/ + https://github.com/robbyrussell/oh-my-zsh/wiki/Themes + https://iterm2colorschemes.com/

---


### 21.6.19
**Interneting Is Hard** (14 chapters)

https://internetingishard.com/html-and-css/


---

### 1.7.19
~~Yearly objectives have been set.~~ (The plans are changed.)

~~1. **AWS Certified Developer – Associate** to get.~~
~~2. Have expertise on **Symfony.**~~


---

### 14.7.19
So far on **Ultimate AWS Certified Developer Associate 2019** on Udemy

https://www.udemy.com/aws-certified-developer-associate-dva-c01/

#### AWS Fundamentals:

- **IAM** (Identity and Access Management)
- **EC2** (Elastic Compute Cloud)

- **ELB** (Elastic Load Balancing)
- **ASG** (Auto Scaling Groups)
- **EBS** (Elastic Block Store)

- **Route 53** (DNS Server)
- **RDS** (Relational Database Service )
- **ElastiCache** (Cache Server)
- **VPC** (Virtual Private Cloud)

- **S3** (Buckets, Storing Service)

- **CLI** (Command Line Interface)
- **SDK** (Software Development Kit)

---

### 15.7.19
**From Zero to App**: One project from start to finish

https://www.youtube.com/watch?v=qaKTmcclmug&list=PLRpq_iSq4KCHOpRymcaj6PMhrX-cLpz6e

- HTML, CSS (Tailwind)
- JS, React, React Router
- GraphQL, Apollo
- IndexedDB
- PWA (Service Workers, Push Notifications, Cache API)
- Node.js, Express, PostgreSQL

---

### 17.7.19
PHPUnit sample **mock builder:**
```
$redirectId = '1';

$mockGeoIpRedirect = $this->getMockBuilder( GeoIpRedirect::class )
  ->disableOriginalConstructor()
  ->setMethods( ['removeRedirectById'] )
  ->getMock();

$mockGeoIpRedirect->expects( $this->once() )
  ->method( 'removeRedirectById' )
  ->with( $redirectId )
  ->willReturn( 0 );

$result = $mockGeoIpRedirect->removeRedirect( $redirectId );
$expected = [
  'type' => 'error',
  'message' => 'Something went wrong with removing the redirect.'
];

$this->assertEquals( $result, $expected );

// Set constructor args
// $mockGeoIpRedirect
//    ->setConstructorArgs( [ $redirectDataToUpdate ] ))

```

---

### 18.7.19
What you need to know to become a **full-stack serverless developer?**

https://www.freecodecamp.org/news/what-you-need-to-become-a-full-stack-serverless-developer/

---

### 29.7.19
React Component Libraries

- **Semantic UI** - https://react.semantic-ui.com/
- **Ant Design of React** - https://ant.design/docs/react/introduce
- **Material UI** - https://material-ui.com/
- **Grommet Design Kit** - https://github.com/grommet/design-kit

React Admin Dashboard Templates

- **Shards Dashboard** - https://designrevision.com/demo/shards-dashboard-lite-react/blog-overview#
- **Devias Kit** - https://react-material-dashboard.devias.io/dashboard
- **CoreUI Dashboard** - https://coreui.io/react/demo/#/dashboard
- **Tabler React** - http://tabler-react.com/

---

### 7.8.19
Indie making communities

- **Maker Mag** - https://makermag.com/
- **Product Hunt** - https://www.producthunt.com/
- **Indie Hackers** - https://www.indiehackers.com/

---

### 10.8.19
**AWS Elastic Beanstalk** Docker Multi Container Deployment

```
Short version with awsebcli

$ eb deploy

Long version

$ zip -r deployment.zip .

$ aws s3 mb s3://test-docker-eb --region eu-west-1

$ aws s3 cp deployment.zip s3://test-docker-eb --region eu-west-1

$ aws elasticbeanstalk create-application-version --application-name test \
    --version-label v1 \
    --source-bundle S3Bucket="test-docker-eb",S3Key="deployment.zip" \
    --auto-create-application \
    --region eu-west-1

$ aws elasticbeanstalk update-environment --application-name test \
    --environment-name stage \
    --version-label v1 --region eu-west-1
```

- https://read.acloud.guru/docker-on-elastic-beanstalk-tips-e1a4e6b70ff2

---

### 12.8.19
**AWS Elastic Beanstalk** Survival Guide (7 chapters)

https://colintoh.com/blog/aws-elastic-beanstalk-survival-guide-introduction

---

### 10.8.19
Just started out with React on a little side project. Here comes the **Euphony!**

https://github.com/ebru/euphony

---

### 18.8.19
Complete **React** Developer in 2019 (w/ Redux, Hooks, GraphQL)

https://www.udemy.com/complete-react-developer-zero-to-mastery/

---

### 29.8.19
**What is the difference between Docker and Virtual Machines?**

In docker, isolation is done on the kernel level without the need for a guest operating system. It shares the host operating system.

**What is the relation between Docker and Kubernetes?**

Kubernetes is a container orchestration system for Docker containers and uses pods which include one container or more. Kubernetes is a tool that coordinates and schedules containers, solves how different containers communicate with each other and how can container instances be scaled.

**What is the difference between imperative and declarative deployments?**

In imperative deployments, you say what to do, decide on current states and all steps to do.
In declarative deployments, you say what you need in a config file and a tool does it for you. (Like the master in k8s.) It is done somehow and you do not care about previous steps.

---

### 31.8.19
**Creating a Side Project**, eBook (8 Stages, 43 Strategies & 59 Tools)

A practical guide on how to become a Viking and beat every problem you will face when building a side project.

https://www.failory.com/side-project

---

### 1.10.19
**GraphQL Tutorial**, by Net Ninja

https://www.youtube.com/playlist?list=PL4cUxeGkcC9iK6Qhn-QLcXCXPQUov1U7f


---

### 2.10.19
- **Algorithms and Data Structures, again!** JavaScript Algorithms and Data Structures Masterclass on Udemy

https://www.udemy.com/course/js-algorithms-and-data-structures-masterclass/learn/

- Find the **execution time of a function** in JS

```
console.time();
function();
console.endTime();

// [ 70 ]
default: 10.331ms
```

On browser:
```
let t1 = performance.now();
function();
let t2 = performance.now();

console.log(`Time elapsed: ${(t2 - t1)/1000} seconds`);
```

---

### 7.10.19
**Create self signed ssl certificate** for development purposes using OpenSSL

```
$ openssl version

$ openssl genrsa 2048 > privatekey.pem

$ openssl req -new -key privatekey.pem -out csr.pem

$ openssl x509 -req -days 365 -in csr.pem -signkey privatekey.pem -out public.crt
```

```
$ openssl req -x509 -out localhost.crt -keyout localhost.key \
  -newkey rsa:2048 -nodes -sha256 \
  -subj '/CN=localhost' -extensions EXT -config <( \
   printf "[dn]\nCN=localhost\n[req]\ndistinguished_name = dn\n[EXT]\nsubjectAltName=DNS:localhost\nkeyUsage=digitalSignature\nextendedKeyUsage=serverAuth")
```

---

### 18.10.19
**Cookies vs Tokens**

- https://dzone.com/articles/cookies-vs-tokens-the-definitive-guide

- https://stackoverflow.com/questions/17000835/token-authentication-vs-cookies

- https://scotch.io/bar-talk/why-jwts-suck-as-session-tokens

---

### 21.10.19
**XSS: Cross-site scripting attacks**

Injecting a malicious script into trusted websites.

```
<script>alert('hello');</script>
```

Injecting through input fields etc. React prevents this as default while permitting setting innerHTML directly.

1. Escaping
2. Validating input
3. Sanitizing
4. CSP (Content security policy)

*"If an attacker can execute code on your domain, your JWT tokens are vulnerable. Our CTO has argued in the past that XSS attacks are much easier to deal with compared to XSRF attacks because they are generally better understood. Many frameworks, including Angular, automatically sanitize inputs and prevent arbitrary code execution." dzone*

**XSRF: Cross-site request forgery**

An attack that forces an end user to execute unwanted actions on a web application in which they're currently authenticated.

1. Check for the request if it comes from the same origin. CORS.
2. A signed token must be provided in the request. JWT.

*"Cross Site Request Forgery attacks are not an issue if you are using JWT with local storage. On the other hand, if your use case requires you to store the JWT in a cookie, you will need to protect against XSRF. XSRF are not as easily understood as XSS attacks." dzone*

---

### 22.10.19
Four Principles of **Object-Oriented Programming**

**1. Encapsulation**

It makes all objects manage their state on their own with private variables/methods and only expose some public functionality to other classes. They can use these public methods to modify or reach the state but they can never directly change it.


**2. Polymorphism**

Polymorphism means `many shapes` in Greek. Polymorphism gives a way to use a class exactly like its parent so there’s no confusion with mixing types. But each child class keeps its own methods as they are.

This typically happens by defining a (parent) interface or abstract class to be reused. It outlines a bunch of common methods. Then, each child class implements its own version of these methods and we treat them like the same type of object.

ex.`Figure Interface` lets you create a list of mixed `triangles`, `circles`, and `rectangles`. You can define it once and accept a `Figure` as an argument. Whether you pass a triangle, circle or rectangle — as long as they implement `CalculatePerimeter()`, their type doesn’t matter.

**3. Inheritance**

It makes us able to share common logic between classes using a child/parent hierarchy. A child can use all functions from its parent and also implement its own unique logic addition to this. This way, we can prevent repetitions on the codebase.


**4. Abstraction**

Hides all internal implementation details. It only reveals the high order operations to other classes and it makes a lot of work under the hood that we do not need to care for. Implementations can change through time but it does rarely affect the abstractions we use.

https://www.freecodecamp.org/news/object-oriented-programming-concepts-21bb035f7260/

Just to remember this easily; **E**ncapsulation **P**olymorphism **I**nheritance ~~**C**~~ **A**bstraction, EPICA.

---

### 23.10.19
**Override hash and equals method**

We can override the equals and hash method of a key object to determine how the hash code is generated and when two key objects should be considered equal. This way, we can come up with a custom hash behavior.

`obj1 = Example('test')`

`obj2 = Example('test')`

`obj1` does not equal `obj2` since they are completely new objects by reference and they will have different hashes as default. But if we modify hash functionality like below, they will be treated as the same by hash map/dict.

```
class Example:
  def __init__(self, x):
    self.x = x

  def __hash__(self):
    # Hash by the value of x
    return hash(self.x)
 
  def __eq__(self, other):
    return (
      self.__class__ == other.__class__ and
      # Compare the values of x to determine the equality
      self.x == other.x
    )
```

https://hynek.me/articles/hashes-and-equality/

https://stackoverflow.com/questions/390250/elegant-ways-to-support-equivalence-equality-in-python-classes


---

### 25.10.19
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@

**@    WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED!     @**

@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@

ECDSA host key for `'your server hostname or ip'` has changed and you have requested strict checking.

Use ssh-keygen to delete the invalid key.

```
$ ssh-keygen -R 'your server hostname or ip'
```

https://www.digitalocean.com/community/questions/warning-remote-host-identification-has-changed

---

### 26.10.19
How to Learn **Software Design and Architecture** - a Roadmap

https://www.freecodecamp.org/news/software-design/

---

### 27.10.19
GraphQL Queries with **Apollo React Hooks**

```
import { useQuery } from '@apollo/react-hooks';
import gql from 'graphql-tag';

const GET_USER = gql`
    query getUser($userId: ID!) {
        getUser(userId: $userId) {
            name
        }
    }
`;

const UserProfile = ({ userId }) => {
  const { data, loading, error } = useQuery(
      GET_USER,
      { variables: { userId } }
  );

  if (loading) return <Spinner />;
  if (error) return <p>Error: {error.message}</p>;

  const { name } = data.getUser;

  return (
    <h1>{name}</h1>
  )
}
```

https://blog.apollographql.com/apollo-client-now-with-react-hooks-676d116eeae2

---

### 12.11.19
**1. Bubble Sort** // Sorting Algorithms

A sorting algorithm where the largest values bubble up to the top. Loop from the beginning while comparing/swaping each item on each iteration.

`[1, 7, 3, 4, 11, 4, 5]`

`[1, 3, 4, **7**, 4, 5, **11**]`

`[1, 3, 4, 4, 5, **7**, **11**]`

```
// optimized
const bubbleSort = arr => {
  for (let i = arr.length; i > 0; i--) {
    let noSwaps = true;
    for (let j = 0; j < i - 1; j++) {
      console.log(arr, arr[j], arr[j+1]);
      if (arr[j] > arr[j+1]) {
        // swap
        let temp = arr[j];
        arr[j] = arr[j+1];
        arr[j+1] = temp;
        noSwaps = false;
      }
    }
    if (noSwaps) break;
    console.log('one pass completed.');
  }
  return arr;
}

// not optimized
const bubbleSort = arr => {
  for (let i = 0; i < arr.length; i++) {
    for (let j = 0; j < arr.length; j++) {
      if (arr[j] > arr[j+1]) {
        // swap
        let temp = arr[j];
        arr[j] = arr[j+1];
        arr[j+1] = temp;
      }
    }

  }
  return arr;
}
```

---

### 13.11.19
DDD: **Domain-Driven Design**

A domain-driven design architecture is designed to grow incrementally over time. The domain influences the system, the system influences the domain. There is a cycle.

**1. Collaborative**

```
"Business people and developers must work together daily through the project."
- Agile Manifesto
```

**2. Modeling**

Structure of the code models one-to-one to the structure of the domain. All collaborators can make sense of the structure. Changes are made to the domain, which maps to where code changes should occur.

**3. DDD Is Incremental**

Come up with only enough architecture to solve the immediate problem. The code evolves as you learn more about the problem and more architecture is added.

- Make a small change and release.
- Assess (feedback).
- Inspect and adapt.
- Improve.

Stories in agile describe end user performing a domain-driven, result-oriented task, **your user’s** work.

**Microservices.** Every entity should be associated with one context with their own properties.

ex. Store and Warehouse should have Product entity differently.

Store -> `Product (shelf, size, weight)` // Warehouse -> `Product (image, price)`

- Move away from relational database thinking.
- Bad to have single product object in multiple contexts.

Everything stays context specific.

**Reactive vs Declarative Systems.** When an order is placed;

In **declarative systems**, Shopping service tells Billing, Warehouse and Email services what to do directly and is aware of their existences. There is a tight relationship between services.

`issueInvoice()` to Billing, `queueItem()` to Warehouse, `emailCustomer()` to Email.

In **reactive systems**, Shopping service fires an event and does not care about which systems will use it. It eliminates coupled relationships between downstream and upstream services.

`orderPlaced()` is fired to announce an order is placed. Any related service will handle the next on their own with publish-subscribe model.

In DDD, the majority of communication between entities should be a reactive model and best way to do this to use a messaging system like **Kafka**, **RabbitMQ**.

https://www.linkedin.com/learning/software-architecture-domain-driven-design/

---

### 26.11.19

```
"Just enjoy your tea and a cookie.
And be nice to the people around you.
That's all there is.
Everything else is just filling time."
```

---

### 01.12.19
- The Modern **GraphQL Bootcamp** (with Node.js and Apollo)

https://www.udemy.com/course/graphql-bootcamp/

- C4n y0u H4ck 1t 👾 - The AIS Hacking Challenge

https://hack.ainfosec.com/

- **Advent of Code**: 2019

This is an Advent calendar of small programming puzzles for a variety of skill sets and skill levels that can be solved in any programming language you like. It takes place each year starting on 1st of December.

https://adventofcode.com/2019/

---

### 07.12.19
Asynchronous with **Redux Saga**

Sagas intercept actions with side effects and handle them, Redux reducers remain pure. Redux Saga utilizes ES6 generator functions for this. Generators allow for synchronously written asynchronous code. 

A generator will automatically pause - or yield - at each asynchronous call until it completes before continuing. This paradigm allows for much simpler and more readable code by centralizing asynchronous logic for more manageable and sophisticated async flows.

 **fork** → Performs a non-blocking operation on the function passed.

 **take** → Pauses until action received.

 **race** → Runs effects simultaneously, then cancels them all once one finishes.

 **call** → Runs function. If it returns a promise, pauses the Saga until resolved.

 **put** → Dispatches an action.

 **select** → Runs a selector function to get data from the state.

 **takeLatest** → Executes the operation, returns only the results of the last call.

 **takeEvery** → Will return results for all the calls triggered.

https://dev.to/irmerk/asynchronous-with-redux-sagas-44dm

---

### 12.12.19
**Waiting for user to stop typing** on handling input changes / React

```
const ChooseUsername = () => {
  const [username, setUsername] = useState('ebru')
  
  const checkUsername = username => {
    if (username !== 'ebru') {
      setCheckIcon(availableState)
    } else {
      setCheckIcon(alreadyTakenState)
    }
  }
  
  useEffect(() => {
    const timeout = setTimeout(() => {
      console.log('username', username)
      checkUsername(username)
    }, 500)

    return () => clearTimeout(timeout)
  }, [username])
  
  ...
  
  <FormInput
    type='text'
    value={username}
    onChange={event => setUsername(event.target.value)}
    label='Username'
    required
  />
  
  ...
}
```

---

### 22.12.19
Web development, **illustrated.** Illustrated Explainers & Sketchnotes

https://illustrated.dev/
