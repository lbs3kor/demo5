pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    if (isUnix()) {
                        sh 'nohup ./some_script.sh &'
                    } else {
                        bat 'start some_script.bat'
                    }
                }
            }
        }
    }
}
