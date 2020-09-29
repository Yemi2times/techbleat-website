pipeline {
    agent any 
    stages {
  
        stage ('Code Download') {
            steps {
                echo "Hey, i'm about to download"
                git 'https://github.com/Yemi2times/techbleat-website.git'
            }
        }
        stage ('Copy index file') {
            steps {
                echo "copying index file"
                sh 'sudo cp index.html  /usr/share/nginx/html'
            }
        }
        stage ('Copy jpeg file') {
            steps {
                echo "copying jpeg file"
                sh 'sudo cp devops.jpg /usr/share/nginx/html '
            }
        }
    }
}
