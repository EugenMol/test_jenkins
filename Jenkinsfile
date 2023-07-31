pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo "---Checkout----"
                git url: "https://github.com/EugenMol/test_jenkins.git", branch: "main"
                sh '''
                ls -la
                
                
                '''
                }
            }
        stage('Check_Dockerfike') {
            steps {
                echo "-----Check_Dockerfike-----"
                sh '''
                    docker info
                    docker run --rm -i hadolint/hadolint < Dockerfile
                    echo $?
                '''
            }
        }
        stage('Test'){
            steps {
               echo "-----Test------"
            }
        }
        stage('Deploy') {
            steps {
                echo "-----Deploy----"
            }
        }
    }
}
