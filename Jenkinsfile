pipeline {
    agent any 
    stages {
        stage ('Build') {
            steps {
                sh 'g++ -o PES2UG20CS579-1 hello.cpp'
            }
        }
        stage ('Test') {
            steps {
                h './PES2UG20CS579-1'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
