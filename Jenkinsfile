pipeline {
    agent any
    parameters {
        string(name: 'PERSON', defaultValue: 'syam', description: 'Who should I say hello to?')
    }
    stages {
        stage('Example') {
            steps {
                echo "Hello ${params.PERSON}"
            }
        }
    }
    
  parameters { 
      booleanParam(name: 'DEBUG_BUILD', defaultValue: true, description: '')
  }
  parameters { 
        choice(choices: ['Active', 'Inactive'], description: '', name: 'Choice')
  }
}pa
