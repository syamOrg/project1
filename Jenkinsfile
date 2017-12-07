properties([parameters([choice(choices: ['Active', 'Reactive', 'InActive'], description: 'activity', name: 'choice'), booleanParam(defaultValue: true, description: 'Boolean Parameter', name: 'Boolean'), string(defaultValue: 'Syam', description: '', name: 'String ')]), pipelineTriggers([githubPush()])])
pipeline {
    agent any
        stages {
            stage('Build') {
                when {
                    expression {
                        "foo" == "bar"
                    }
                }
                steps {
                    echo 'Building'
                }
            }
        stage('Test') {
            when {
                environment name: 'JOB_NAME', value: 'foo'
            }
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            when {
                branch 'master'
            }
            steps {
                echo 'Deploying...gd...'
            }
        }
    
     stage('Deployed') {
            when {
                branch 'master'
            }
            steps {
                echo 'Deployed'
            }
        }
    }
}
