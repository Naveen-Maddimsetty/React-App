pipeline {
  agent any
     stages {
      stage("Clone") {
            steps { 
                sh "https://github.com/Naveen-Maddimsetty/React-App.git"
            }
        }
        stage("Build") {
            steps { 
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
