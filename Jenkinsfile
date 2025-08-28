pipeline {
    agent any

    stages {
        stage('compile') {
            steps {
                echo 'Hello built stage'
                sh 'mvn compile'
            }
        }
        stage('test'){
            steps{
                echo "hello test stage"
                sh 'mvn test'
            }
        }
        stage('package') {
            steps {
                echo 'Hello pacakage stage'
                sh 'mvn package'
            }
        }
        stage('deploy'){
            steps{
                echo "hello deploy stage"
                sh 'python3 addition.py'
            }
        }
    }
}
