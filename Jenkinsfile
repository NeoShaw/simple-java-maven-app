pipeline {
    agent {
        docker {
            image 'maven:3.5-jdk-8-onbuild-alpine'
            args '-v /Users/yichuan/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}
