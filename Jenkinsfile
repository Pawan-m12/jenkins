pipeline {
    agent any 
    parameters {
        choice(name: 'STAGE_NAME', choices: ['STAGE-1', 'STAGE-2'], description: 'Enter stage name to execute ?')
    }
    stages {
        stage('STAGE-1') {
            when { 
                expression{ params.STAGE_NAME == "STAGE-1" }
            }    
            steps{
                print "DEBUG: parameter STAGE_NAME = ${params.STAGE_NAME}"
            }
        }

        stage('STAGE-2'){
            when { 
                expression{ params.STAGE_NAME == "STAGE-2" }
            }    
            steps{
                print "DEBUG: parameter STAGE_NAME = ${params.STAGE_NAME}"
            }    
        }
    }
}
