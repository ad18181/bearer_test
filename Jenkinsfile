pipeline {

    agent {

        docker {image 'bearer/bearer:latest '}
    }

 

    stages {

        stage('Checkout') {

            steps {

                // Checkout code from the branch

                checkout scm

            }

        }

 

        stage('Code Analysis with Horusec') {

            steps {

                script {

                    sh 'bearer version '

                }

            }

        }

    }

}
