pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "this is build stage"
            }
        }
        stage('Test') {
            steps {
                echo "this is test stage"
            }
        }
        stage('Deploy') {
            when { tag "release-*" }
            steps {
                echo 'Deploying only because this commit is tagged...'
               
            }
        }
    }
}
