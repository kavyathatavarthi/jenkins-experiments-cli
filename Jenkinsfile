pipeline {
    agent any
    stages {
        stage('Version 1') {
            steps {
                echo 'Pipeline execution has started.'
                // Task 2: Display workspace via env variable
                echo "Workspace Path: ${env.WORKSPACE}"
            }
        }
        stage('Version 2 - File Listing & Time') {
            steps {
                echo 'Starting Version 2 Tasks...'
                
                // Task 2: List all files and folders in the workspace
                bat 'dir'
                
                // Task 3: Display current system time
                bat 'time /t'
            }
        }
        stage('Version 3') {
            steps {
                // Task 2 & 3: Create file and write message
                bat 'echo Simple build message > buildlog.txt'
                bat 'type buildlog.txt'
            }
        }
    }
}
