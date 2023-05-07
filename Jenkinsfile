pipeline {
    agent any
    triggers {
        pollSCM('H/1 * * * *') // Polls the SCM every 15 minutes
    }
    stages {
        stage('Build') {
            steps {
                echo "${env.GIT_BRANCH}"
                echo "${env.BRANCH_NAME}"
            }
        }
        // Additional stages
    }
    


def branchCreated = sh(returnStdout: true, script: 'git show-ref --heads') 
if (branchCreated.contains('refs/heads/new-branch')) {
    // Actions to perform when a new branch is created
    // For example, you can trigger a specific stage or run a set of steps here.
}
