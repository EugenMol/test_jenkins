pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo "---Checkout----"
                dir("testgit") {
                git(
                    url: "git@github.com:EugenMol/test_jenkins.git",
                    branch: "main",
                    changelog: true,
                    poll: true
                    )
                    }
                }
            }
        stage('Build') {
            steps {
                echo "-----Build-----"
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
