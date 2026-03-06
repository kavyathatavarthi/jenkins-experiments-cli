pipeline {
    agent any
    stages {
        stage('Version 1') {
            steps {
                echo 'Pipeline execution has started.'
                echo "Workspace Path: ${env.WORKSPACE}"
            }
        }
        stage('Version 2 - File Listing & Time') {
            steps {
                echo 'Starting Version 2 Tasks...'
                
                bat 'dir'
                
                bat 'time /t'
            }
        }
        stage('Version 3') {
            steps {
                bat 'echo Simple build message > buildlog.txt'
                bat 'type buildlog.txt'
            }
        }
        stage('Version 4') {
            steps {
                bat "echo Jenkins Build Number: ${env.BUILD_NUMBER} >> buildlog.txt"
                echo "--- Updated Log Contents ---"
                bat 'type buildlog.txt'
            }
        }
    }
}
