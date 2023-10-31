pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                bat "npm install"
                bat "npm run build"
            }
        }
        stage("Test") {
            steps {
                bat "npm run test"
            }
        }
        stage("Deploy") {
            steps {
                bat "cp -r C:/ProgramData/Jenkins/.jenkins/workspace/reactwebapplication/build  C:/Users/Matoshri/Downloads/nginx-1.24.0/nginx-1.24.0/"
            }
        }
    }
}
