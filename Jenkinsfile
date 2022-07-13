pipeline {
    agent any
    stages {
        stage ('Git Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Rameshagwd/Nexus_Repo_Pipeline.git'
            }
        }

        stage ('MVN Clean') {
            steps {
                sh 'mvn clean'
            }
        }

        stage ('MVN Compile') {
            steps {
                sh 'mvn compile'
            }
        }

        stage ('MVN install') {
            steps {
                sh 'mvn install'
            }
        }

        stage ('MVN validate') {
            steps {
                sh 'mvn install'
            }
        }

        stage ('MVN package') {
            steps {
                sh 'mvn package'
            }
        }

        stage ('MVN test') {
            steps {
                sh 'mvn test'
            }
        }

        stage ('MVN Deploy') {
            steps {
                sh 'mvn deploy'
            }
        }
    }
}