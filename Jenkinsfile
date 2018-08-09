#!/usr/bin/env groovy
pipeline {
  agent any
  stages {
    stage('dsl') {
      steps {
        jobDsl targets: ['jobs/*.groovy'].join('\n'),
               removedJobAction: 'DELETE',
               removedViewAction: 'DELETE,
               lookupStrategy: 'SEED_JOB',
               sandbox: true
      }
    }
  }
}

/*
node {
    jobDsl targets: ['jobs/*.groovy'].join('\n'),
           ignoreMissingFiles: true,
           removedJobAction: 'DELETE',
           removedViewAction: 'DELETE',
           lookupStrategy: 'JENKINS_ROOT',
           sandbox: true
    step([
        $class: 'ExecuteDslScripts',
        targets: ['jobs/*.groovy'].join('\n'),
        removedJobAction: 'DELETE',
        removedViewAction: 'DELETE',
        lookupStrategy: 'SEED_JOB',
        additionalParameters: [message: 'Hello from pipeline', credentials: 'SECRET']
    ])
}
*/
