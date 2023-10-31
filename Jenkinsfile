pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                bat "sudo npm install"
                bat "sudo npm run build"
            }
        }
        stage("Test") {
            steps {
                bat "sudo npm run test"
            }
        }
        stage("Deploy") {
            steps {
                bat "sudo cp -r C:\ProgramData\Jenkins\.jenkins\workspace\reactwebapplication C:\Users\Matoshri\Downloads\nginx-1.24.0\nginx-1.24.0"
            }
        }
    }
}
