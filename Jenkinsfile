pipeline {
    agent any
    stages {
        stage('Build & Test') {
            steps {
                // Maven Wrapper ile test
                sh './mvnw clean test'
            }
        }
        stage('Deploy') {
                    steps {
                        // Maven Wrapper ile test
                    }
                }
    }
    post {
        always {
            // Test sonuçlarını archive et
            junit '**/target/surefire-reports/*.xml'
        }
    }
}
