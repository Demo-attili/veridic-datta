#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/Demo-attili/veridic-atl'],
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
        stage('Checkout') {
            steps {
                echo 'checkout step'
            }
        }
		
        stage('Build') {
            steps {
                
                    echo 'Build step'
                
            }
       	   }
		   
       
	   stage('Deploy'){
	       steps {
		   echo 'deploy step'
	   }
	   }
	   
	   
    }
}
