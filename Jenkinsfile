pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ temp.cpp -o temp'
                 build job: 'PES1UG20CS237-1', wait: false
                 echo 'Build is successful -Yuktha'
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp.cpp'
                echo 'Testing -Yuktha'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy is successful -Yukha'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
