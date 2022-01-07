pipeline {
    agent none
    stages {
        stage('PythonImage') {
            agent {
                docker {
                    image 'python:latest'
                }
            }
            steps {
                sh 'python --version'
            }
        }
        stage('PostgresImage') { 
            agent {
                docker {
                    image 'postgres:latest' 
                }
            }
            steps {
                sh 'postgres -V' 
            }
        
        }
	stage('Sqlimage') { 
            agent {
                docker {
                    image 'mysql:5.6' 
                }
            }
            steps {
                sh 'mysql -V' 
            }
        
        }
    }
}
