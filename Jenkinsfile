pipeline {
     agent any
     stages {
        stage("Build") {
            steps { 
                sh "https://github.com/Naveen-Maddimsetty/React-App/"
                sh "npm install"
                sh "npm run build"
            }
        }
        stage("Test") {
            steps {
                sh "npm run test"
            }
        }
        stage("Deploy") {
            steps {
                sh "cp -r C:/ProgramData/Jenkins/.jenkins/workspace/reactwebapplication/build  C:/Users/Matoshri/Downloads/nginx-1.24.0/nginx-1.24.0/"
            }
        }
    }
}
