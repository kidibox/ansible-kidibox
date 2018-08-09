node {
    jobDsl scriptText: 'job("example-2")'

    jobDsl targets: ['jobs/common.groovy'].join('\n'),
           removedJobAction: 'DELETE',
           removedViewAction: 'DELETE',
           lookupStrategy: 'SEED_JOB'
}
