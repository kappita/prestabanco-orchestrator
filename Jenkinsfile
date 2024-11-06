pipeline {
    agent any

    stages {
        stage('Trigger Pipelines') {
            parallel {
                stage('Trigger Pipeline 1') {
                    steps {
                        script {
                            // Replace 'pipeline1-job-name' with the actual name of the first pipeline/job
                            build job: 'prestabanco-backend', wait: true, propagate: true
                        }
                    }
                }
                stage('Trigger Pipeline 2') {
                    steps {
                        script {
                            // Replace 'pipeline2-job-name' with the actual name of the second pipeline/job
                            build job: 'prestabanco-frontend', wait: true, propagate: true
                        }
                    }
                }
            }
        }
    }
}
