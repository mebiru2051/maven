pipeline {
    agent {
        label 'maven'
    }
    tools {
        jdk 'openjdk8'
        maven 'maven363'
    }
    stages {
        stage('Build') {
            steps {
                sh "mvn clean compile"
        }
    }
}
post {
    success {
        echo"good job"
    }
    failure {
            echo "improve the skills"
    }
    always {
            echo "work hard"
        }
    }
}