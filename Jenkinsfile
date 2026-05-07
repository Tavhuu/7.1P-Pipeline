pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Task: Compiling and packaging the application source code into a deployable artifact.'
                echo 'Tool: Maven - automates the build process by compiling source code and packaging it into a JAR/WAR file.'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Task: Running unit tests to verify individual functions and integration tests to ensure components work together.'
                echo 'Tools: JUnit for unit testing, Selenium for integration testing.'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Task: Analysing source code to ensure it meets industry coding standards and best practices.'
                echo 'Tool: Checkstyle - analyses Java code style and flags violations against defined coding rules.'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Scanning code and dependencies for known security vulnerabilities and CVEs.'
                echo 'Tool: OWASP Dependency-Check - identifies vulnerable open-source dependencies in the project.'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploying the packaged application to a staging server for pre-production verification.'
                echo 'Tool: AWS CLI - used to deploy the application to an AWS EC2 staging instance.'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Running integration tests on the staging environment to validate the application in a production-like setting.'
                echo 'Tool: Selenium WebDriver - automates browser-based integration tests against the staging server.'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploying the fully verified application to the live production server.'
                echo 'Tool: AWS CLI - used to deploy the application to an AWS EC2 production instance.'
            }
        }

    }
}
