pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'py -m pip install --break-system-packages -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'py -m pytest'
            }
        }
    }
}