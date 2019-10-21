# notes from the day.
This is a little diary for me to track the progress and learning.

### 25.5.19
- Created a web development learning roadmap.

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
Yearly objectives has been set.

1. **AWS Certified Developer – Associate** to get.
2. Have expertise on **Symfony.**


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

- **Grommet Design Kit** - https://github.com/grommet/design-kit
- **Ant Design of React** - https://ant.design/docs/react/introduce
- **Material UI** - https://material-ui.com/

React Admin Dashboard Templates

- **Shards Dashboard** - https://designrevision.com/demo/shards-dashboard-lite-react/blog-overview#
- **Antd Admin** - https://antd-admin.zuiidea.com/en/dashboard
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

In docker, isolation is done on the kernel level without the need for a quest operating system. It shares the host operating system.

**What is the relation between Docker and Kubernetes?**

Kubernetes is a container orchestration system for Docker containers and uses pods which include one container or more. Kubernetes is a tool that coordinates and schedules containes, solves how different containers communicate each other and how can container instances be scaled.

**What is the difference between imperative and declarative deployments?**

In imperative deployments, you say what to do, decide on current states and all steps to do.
In declarative deployments, you say what you need in a config file and a tool does it for you. (Like master in k8s.) It is done somehow and you do not care about previous steps.

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
- **Algorithms and Data Structures, Again!**, JavaScript Algorithms and Data Structures Masterclass on Udemy

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

---

### 18.10.19
**Cookies vs Tokens**

- https://dzone.com/articles/cookies-vs-tokens-the-definitive-guide

- https://stackoverflow.com/questions/17000835/token-authentication-vs-cookies

- https://scotch.io/bar-talk/why-jwts-suck-as-session-tokens

---

### 21.10.19
**XSS**: Cross-site scripting attacks
Injecting a malicious script into trusted websites.

```
<script>alert('hello);</script>
```

Injecting through input fields etc. React prevents this as default while permitting setting innerHTML directly.

**CSRF**: Cross-site request forgery
An attack that forces an end user to execute unwanted actions on a web application in which they're currently authenticated.

1. Check for the request if it comes from the same origin. CORS.
2. Signed token must be provided in the request. JWT.
