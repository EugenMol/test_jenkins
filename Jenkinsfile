pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo "---Checkout----"
//                sh "git clone git@github.com:EugenMol/Md-SA2-24-23.git"
//                 dir("testgit") {
//                 git(
//                     url: "git@github.com:EugenMol/Md-SA2-24-23.git",
//                     branch: "master",
//                     changelog: true,
//                     poll: true
//                     )
//                     }
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
