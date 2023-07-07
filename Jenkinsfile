pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
              git branch: 'main', url: 'git@github.com:sivaram2662/node-js-web-application.git'
            }
        }
        stage('node') {
            steps {
              sh 'sudo yum install nodejs -y'
            }
        }
        stage('npm') {
            steps {
              sh 'curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash'
            }
        }
         stage('nvm') {
            steps {
              sh '. ~/.nvm/nvm.sh'
            }
        }
         stage('nvm1') {
            steps {
              sh 'npm install'
            }
        }
    }
}
