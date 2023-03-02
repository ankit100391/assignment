pipeline {
    agent any 
    stages {
        stage('STAGE-1') {
            when {
                branch 'master'
            }
            steps{
                sh "echo STEGE-2 executes if branch is master"
            }
        }

        stage('STAGE-2'){
            when {
                branch 'test'
            }
            steps{
                sh "echo STEGE-2 executes if branch is master"
            }
        }
    }
}
