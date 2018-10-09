pipeline {
    agent any
        stages {
            stage('compile stage') {
                steps {
                withmaven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn clean compile'
            }
                }
       stage('test stage') {
           steps {     
           withmaven (maven : 'Apache Maven 3.5.2')
                    sh 'mvn testing'
            }
       }
        stage('deploy stage') {
            steps {
                withmaven (maven : 'Apache Maven 3.5.2')
                    echo 'mvn deploy'
            }
        }
        }
}
