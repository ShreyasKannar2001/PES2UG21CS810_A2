pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG21CS818-1 new.cpp'
                echo "Build Successful!!"
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG21CS818-1'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed successfully'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
