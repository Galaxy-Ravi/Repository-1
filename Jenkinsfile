#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/Galaxy-Ravi/Repository-1'],
    pipelineTriggers([upstream(
      threshold: 'SUCCESS',
      upstreamProjects: 'https://github.com/Galaxy-Ravi/Repository-2'
    )])])

pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('Test'){
            steps {
                sh 'java -version'
                
            }
        }
        stage('Deploy') {
            steps {
                sh 'ls'
                sh 'pwd'
            }
        }
    }
}
