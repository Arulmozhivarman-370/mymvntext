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
                sh 'java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App'
            }
        }
    }
}
