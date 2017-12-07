#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/demo-org-project/compile'],
    pipelineTriggers([githubPush()])])

pipeline {
    agent any 

    stages {
        stage('compile') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('install'){
            steps {
                sh 'java -version'
                
            }
        }
        stage('test') {
            steps {
                sh 'ls'
                sh 'pwd'
            }
        }
    }
}
