#!/bin/bash
pipeline {
    agent any 
    stages {
        stage('clone repo') { 
            steps {
                bat "git branch: 'main', credentialsId: 'd271284c-7874-4725-ab78-43323f7b8de6', url: 'https://github.com/dharmaraj257/angular-project.git'"
                bat "ng clean -f angular-project"
            }
        }
        stage('build') { 
            steps {
                bat "ng build -f angular-project"
            }
        }
        stage('Serve') { 
            steps {
                bat "cd angular-project -f angular-project"
                bat"ng serve -f angular-project"
            }
        }
    }
}
