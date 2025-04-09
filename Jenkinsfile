pipeline {
    agent any

    stages {
        stage('Checkout from GitHub') {
            steps {
                git 'https://github.com/SddAdln/jenkins-github-python-demo.git'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'python3 -m unittest test_app.py'
            }
        }
    }
}
