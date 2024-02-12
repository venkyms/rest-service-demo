pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout source code from Git
                // git 'https://github.com/venkyms/rest-service-demo.git'
                checkout([$class: 'GitSCM', branches: [[name: 'main']], userRemoteConfigs: [[url: 'https://github.com/venkyms/rest-service-demo.git']]])
            }
        }
        stage('Build') {
            steps {
                // Build the Maven project
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Run tests
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                // Run Ansible playbook to deploy the Spring Boot application
                sh 'ansible-playbook ansible-run-rest-service-demo.yml'
            }
        }
    }
}
