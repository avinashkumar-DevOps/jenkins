pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/avinashkumar-DevOps/jenkins'
            }
        }

        stage('Compile Java Code') {
            steps {
                sh 'javac DevBuild.java'
            }
        }

        stage('Deploy') {
            steps {
                sh 'java DevBuild'
            }
        }
    }
}
