pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the code using a build automation tool (e.g., Maven)...'
                echo 'Preferred tool: Maven'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit tests and integration tests...'
                echo 'Preferred test automation tool: JUnit (for unit tests), Selenium (for integration tests)'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Integrating a code analysis tool (e.g., SonarQube) to analyze the code...'
                echo 'Preferred tool: SonarQube'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Performing a security scan on the code...'
                echo 'Preferred tool: OWASP ZAP (Zed Attack Proxy)'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying the application to a staging server (e.g., AWS EC2 instance)...'
                echo 'Preferred deployment tool: Jenkins Pipeline (with AWS CodeDeploy plugin)'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests on the staging environment...'
                echo 'Preferred tool: Apache JMeter'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploying the application to a production server (e.g., AWS EC2 instance)...'
                echo 'Preferred deployment tool: Jenkins Pipeline (with AWS CodeDeploy plugin)'
                echo "Updating jenkins script"
            }
        }
    }
    post {
        success {
            // Cleanup steps, if any
            emailext body: 'Verifying message', subject: 'Transmission message', to: 'asmigarg903@gmail.com', attachLog:true
        }
    }
}


