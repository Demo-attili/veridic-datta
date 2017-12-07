#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/Demo-attili/veridic-atl/'],
properties([
  pipelineTriggers([
    upstream(
      threshold: 'SUCCESS',
      upstreamProjects: 'https://github.com/Demo-attili/veridic-atl/'
    )
  ])
])


])

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
