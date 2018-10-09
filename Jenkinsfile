pipeline {
    agent any
        stages {
            stage('maven compile') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    echo 'maven compile'
            }
       stage('maven test') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    echo 'maven testing'
            }
        stage('maven deploy') {
                withmaven (maven : 'Apache Maven 3.5.2')
                    echo 'maven deploy'
            }
        }
}
