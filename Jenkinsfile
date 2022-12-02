pipeline {
    
    agent any
    
    parameters {
        booleanParam(name: "RELEASE", defaultValue: false)
    }
    
    stages {

        stage("Build") {
            steps {
                sh "./gradlew build"
            }
        }
        
        stage("Publish") {
            when { expression { params.RELEASE } }
            steps {
                sh "./gradlew release"
            }
        }
    }
}
