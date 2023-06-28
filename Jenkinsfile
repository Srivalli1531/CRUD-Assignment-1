pipeline {
    agent any
    stages {
        stage ('SCM-Checkout'){
            steps{
                //get some code from a GitHub repository
                git 'https://github.com/Srivalli1531/CRUD-Assignment-1.git'
            }
        }
        stage('build') {
            steps {
                //run Maven on a unix agent.
                sh "mvn -Dmaven.test.failure.ignore=true clean package"
                
            }
        }
    }
}
