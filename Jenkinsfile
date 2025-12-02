@Library('sysadmin') _
pipeline {
    agent any
    tools {
        jdk 'jdk11'
        maven 'maven3'
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/mostafa-soliman46/cicd-lab2.git'
            }
        }
        stage('Build & Test') {
            steps {
                buildJava()
                runTests()
            }
        }
        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
