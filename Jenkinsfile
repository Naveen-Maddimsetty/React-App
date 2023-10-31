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
                sh "sudo rm -rf /var/www/jenkins-react-app"
                sh "sudo cp -r /var/lib/jenkins/workspace/ReactWeb/build/ /var/www/jenkins-react-app/"
            }
        }
    }
}
