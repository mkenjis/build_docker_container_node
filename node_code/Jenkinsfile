pipeline {
    agent {
        dockerfile true
    }
    stages {
        stage('Test3') {
            steps {
                sh 'node --version'
                sh 'echo Testing using Docker container !!!'
                sh 'cd test'
				sh 'npm test'
            }
        }
        stage('Run') {
            steps {
                sh 'echo Running Docker container !!!!'
                sh 'node --version'
            }
        }
    }
}