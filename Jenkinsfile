pipeline {
  agent any
     stages {
        stage("Build") {
            steps { 
                sh "sudo npm install"
                sh "sudo npm run build"
            }
        }
        stage("Test") {
            steps {
                sh "sudo npm run test"
            }
        }
        stage("Deploy") {
            steps {
                sh "sudo cp -r C:/ProgramData/Jenkins/.jenkins/workspace/reactwebapplication/build  C:/Users/Matoshri/Downloads/nginx-1.24.0/nginx-1.24.0/"
            }
        }
    }
}
