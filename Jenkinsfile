pipeline {
    agent any

    tools {
     NodeJS 'NodeJS 4.8.6'
           }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'npm clean compile'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'npm test'
            }
        }
        stage('package') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
