pipeline {
    agent any
    stages {
        stage("Test") {
            when {
                branch "release-*"
            }
            steps {
                echo "Hello World!"
            }
        }
    }
}
