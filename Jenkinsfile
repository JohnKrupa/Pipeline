pipeline {
    agent any
        stages {
            stage('compile stage') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn clean compile'
            }
       stage('test stage') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn testing'
            }
        stage('deploy stage') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    echo 'mvn deploy'
            }
        }
}
