pipeline {
    agent any 
    tools {
        maven 'M2_HOME'
    }
    stages{
        stage('check out the code from github') {
        steps{
            git branch: 'main', url: 'https://github.com/devopscbabu/SampleAddressbook.git'
        }
    }
        stage('Build the Code') {
        steps{
            sh 'mvn clean package'
             }
        }
    }
}
