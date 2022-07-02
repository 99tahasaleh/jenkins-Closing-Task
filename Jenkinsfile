pipeline {
    agent any

    stages {
        stage("Build") {
            steps{
                sh 'mvn clean package'
            }
        }

        stage("Save Artifact"){
            steps {
                archiveArtifacts artifacts: 'target/*.jar', followSymlinks: false
                }
            }
        
        
         stage("Slack Notification"){
            steps {
                slackSend baseUrl: 'https://hooks.slack.com/services/', channel: '#jenkins-close-task', color: '439FE0', message: 'nice job !!!!!!!!!!!', tokenCredentialId: 'slack-demo', username: 'javahomecloud'
                }
            }
        
    }

    post {
        success {
            slackSend channel: 'jenkins_closing_task', message: 'Build Success'
        }
         
        failure {
            slackSend channel: 'jenkins_closing_task', message: 'Build Failed'
        }
    }

}
