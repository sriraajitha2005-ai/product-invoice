pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Source code checkout completed'
            }
        }

        stage('Build') {
            steps {
                bat '"C:\\Program Files\\Maven\\apache-maven-3.9.16-bin\\apache-maven-3.9.16\\bin\\mvn.cmd" clean compile'
            }
        }

        stage('Test') {
            steps {
                bat '"C:\\Program Files\\Maven\\apache-maven-3.9.16-bin\\apache-maven-3.9.16\\bin\\mvn.cmd" test'
            }
        }

        stage('Package') {
            steps {
                bat '"C:\\Program Files\\Maven\\apache-maven-3.9.16-bin\\apache-maven-3.9.16\\bin\\mvn.cmd" package'
            }
        }
    }
}
