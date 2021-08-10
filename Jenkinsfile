pipeline {
    agent any
    stages{
        stage('CheckOut Code ') {
           steps {
              checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'github', url: 'https://github.com/avishai201/jenkinspipeline.git']]])
           }
        }
        stage('Init'){
            steps{
                echo 'testig ...'
            }
        }
        stage('Build'){
             steps{
                 sh  'mvn clean package'
             }

        }
        stage('deploy'){
             steps{
                 echo 'codedeploy ...'
             }
        }
    }
}
