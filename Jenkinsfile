pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
                git url: 'https://github.com/srihareeshh/Jenkins2.git', branch: 'main'
            }
        }
        stage('Build') {
            steps {
                /* 
                   echo 3  -> selects '3. Multiply' for the choice input
                   echo 15 -> enters '15' as the first number
                   echo 25 -> enters '25' as the second number
                */
                bat "(echo 3 && echo 15 && echo 25) | python calculator.py"
            }
        }
    }
}