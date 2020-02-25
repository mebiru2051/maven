pipeline {
    agent {
        label 'maven'
    }
    tools {
        jdk 'openjdk8'
        maven 'maven363'
}
stages {
    stage('build') {
        steps {
            sh"mvn clean test"
        }
    }
}
post {
    success {
        echo"good job"
        Failure {
            echo "improve the skills"
        }
        always {
            echo "work hard"
        }
    }
}