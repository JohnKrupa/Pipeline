pipeline {
    agent any
        stages {
            stage('maven compile') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn clean compile'
            }
       stage('maven test') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn testing'
            }
        stage('maven deploy') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    echo 'mvn deploy'
            }
        }
}
