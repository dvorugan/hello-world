pipeline {
    agent any

    stages('CI1') {
       stage(''){
            steps {
                echo "Checkout"
                checkout scm
            }
        }

       stage('build'){
            steps {
                echo "Build"
                sh 'mvn clean package'
            }
        }

        stage('Test'){
            steps {
                echo "Test"
                sh 'mvn test'
            }
        }

    }
}
