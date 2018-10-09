pipeline {
    agent any
        stages {
            stage('compile') {
                steps {
                withmaven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn clean compile'
            }
                }
       stage('test') {
           steps {     
           withmaven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn testing'
            }
       }
        stage('deploy') {
            steps {
                withmaven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn deploy'
            }
        }
        }
}
