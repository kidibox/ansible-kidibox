node {
    jobDsl targets: ['jobs/common.groovy'].join('\n'),
           ignoreMissingFiles: true,
           removedJobAction: 'DELETE',
           removedViewAction: 'DELETE',
           lookupStrategy: 'JENKINS_ROOT',
           sandbox: true
}
