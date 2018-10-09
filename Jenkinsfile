pipeline {
    agent any
        stages {
            stage('compile') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    echo 'maven compile'
            }
       stage('test') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    echo 'maven testing'
            }
        stage('deploy') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    echo 'maven deploy'
            }
        }
}