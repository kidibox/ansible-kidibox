node {
    jobDsl scriptText: 'job("example-2")'

    jobDsl targets: ['jobs/projectA/*.groovy', 'jobs/common.groovy'].join('\n'),
           removedJobAction: 'DELETE',
           removedViewAction: 'DELETE',
           lookupStrategy: 'SEED_JOB',
           additionalParameters: [message: 'Hello from pipeline', credentials: 'SECRET']
}
