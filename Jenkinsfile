pipeline {
    agent any
    parameters {
        string(name: 'Branch', defaultValue: 'default', description: 'Select which branch you want to select')
        booleanParam(name: 'Rebuild_Database', defaultValue: true, description: 'Should we rebuild the database')
         booleanParam(name: 'Deploy', defaultValue: true, description: 'Should we Deploy this application')
        choice(name: 'Environment', choices: 'Integration\nActive\nInactive' , description: 'use for postgress.sh and code deployment')
    }
    stages {
        stage('Example') {
            steps {
                echo "Hello ${params.Branch}"
                echo "Hello ${params.Rebuild_Database}"
                echo "Hello ${params.Deploy}"
                echo "Hello ${params.Environment}" 
            }
        }
    }
}
