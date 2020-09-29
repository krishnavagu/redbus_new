pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                git credentialsId: 'krishnavagu', url: 'https://github.com/krishnavagu/redbus_new.git'
            }
        }
        stage('Maven Job') { 
            steps {
                sh label: '', script: 'mvn clean package'
            }
        }
        stage('Deploy') { 
            steps {
                echo "this is Deploy job"
            }
        }
    }
}
