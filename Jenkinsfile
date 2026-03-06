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
    }
}
pipeline {
    agent any
    stages {
        stage('Version 2') {
            steps {
                // Task 2: List files
                bat 'dir'
                // Task 3: System Time
                bat 'time /t'
            }
        }
    }
}