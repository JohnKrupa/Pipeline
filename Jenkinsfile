pipeline {
    agent any
        stages {
            stage('compile') {
                steps {
                maven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn clean compile'
            }
                }
       stage('test') {
           steps {     
           maven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn testing'
            }
       }
        stage('deploy') {
            steps {
                maven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn deploy'
            }
        }
        }
}
