# Jenkins-Closing-Task

- The app reads the “Breaking News” from this URL :-  http://www.ynet.co.il/Integration/StoryRss2.xml .

- parses and presents the breaking news XML in an HTML Format. 

- The app is built by intellij idea with Java Spring Boot Framework, And BOOTSTRAP front-end framework.


## Run Locally

Clone the project

```bash
  git clone https://github.com/mohamadassi173/Jenkins-Closing-Task   
```

Go to the project directory

```bash
  cd Jenkins-Closing-Task 
```

Build the project

```bash
  mvn clean package  
```

Start the server

```bash
  java -jar ./target/xmltohtml-0.0.1-SNAPSHOT.jar
```


## Website Demo

<img width="600" alt="image" src="https://github.com/99tahasaleh/jenkins-Closing-Task/blob/main/images/ynetnews.png">

## Jenkins pipeline Job

<img width="600" alt="image" src="https://github.com/99tahasaleh/jenkins-Closing-Task/blob/main/images/jenkins.png">

###  Slack notification

<img width="600" alt="image" src="https://github.com/99tahasaleh/jenkins-Closing-Task/blob/main/images/slack.png">







