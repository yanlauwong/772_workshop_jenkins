pipeline {
    agent any
    
    environment {
        NODE_ENV = 'development'
    }

    stages {
        stage('install npm') {
            steps {
                echo 'NPMing'
                bat 'npm install'
            }
        }
        
         stage('Running Test') {
            steps {
                echo 'runing test'
                bat 'npm test'
            }
        }
    }
    
    post {
        success {
            echo 'u tda best'
        }
          failure {
            echo 'u tda worst'
        }
    }
}
