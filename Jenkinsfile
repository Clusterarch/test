pipeline {
    agent {
        docker { image 'node:7-alpine' }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
                sh 'node --version'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
