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

Node{
	stage 'build'
	echo 'build'
	
	stage 'test'
	echo 'test'
	
	stage 'deploy'
	echo 'deploy'
}
