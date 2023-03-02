pipeline {
    agent any 
    stages {
        stage('parallel') {
            parallel {
                stage('STAGE-1') {
                    when {
                        branch 'main'
                    }
                    steps{
                        sh "echo STAGE-2 executes if branch is main"
                    }
                }

                stage('STAGE-2'){
                    when {
                        branch 'main'
                    }
                    steps{
                        sh "echo STEGE-2 executes if branch is main"
                    }
                }
            }    
        }    
    }
}
