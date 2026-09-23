pipeline {
    agent any

    tools {
        maven 'Maven-3.9.15'
    }

    stages {

        stage('Run Python') {
            steps {
                bat '"C:/Users/DELL/AppData/Local/Programs/Python/Python313/python.exe" hello.py'
            }
        }

        stage('Maven Version') {
            steps {
                bat 'mvn -version'
            }
        }

        stage('Maven Build') {
            steps {
                bat 'mvn clean package'
            }
        }
    }
}
