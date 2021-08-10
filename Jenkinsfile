pipeline {
    agent any
    stages{
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
