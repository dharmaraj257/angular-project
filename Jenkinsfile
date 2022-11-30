pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git  'https://github.com/dharmaraj257/angular-project.git'
                echo "ng build angular-project"
            }
        stage('Post') {
            steps {
                echo "ng serve"
            }
        } 
    }
}
