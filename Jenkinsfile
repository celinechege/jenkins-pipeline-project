pipeline {
    agent any

    triggers {
        pollSCM('H/5 * * * *')
    }

    stages {

        stage("Build") {
            steps {
                sh "echo 'Using Maven to compile and package the Java application'"
            }
        }

        stage("Unit and Integration Tests") {
            steps {
                sh "echo 'Using JUnit for unit testing and TestNG for integration testing'"
            }
        }

        stage("Code Analysis") {
            steps {
                sh "echo 'Using SonarQube to analyse code quality and ensure it meets industry standards'"
            }
        }

        stage("Security Scan") {
            steps {
                sh "echo 'Using OWASP Dependency-Check to scan for known security vulnerabilities in project dependencies'"
            }
        }

        stage("Deploy to Staging") {
            steps {
                sh "echo 'Deploying to a staging environment hosted on an AWS EC2 instance using Ansible'"
            }
        }

        stage("Integration Tests on Staging") {
            steps {
                sh "echo 'Running Postman/Newman integration tests in the staging environment'"
            }
        }

        stage("Deploy to Production") {
            steps {
                sh "echo 'Deploying the application to the production server on AWS EC2 using Ansible'"
            }
        }
    }
}
