pipeline {
    agent any
    triggers {
        // Git branch create trigger
        changeset("[[event=branchCreated]]") {
            // Actions to perform when a new branch is created
            // For example, you can trigger a specific stage or run a set of steps
            // within this block.
        }
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
    post {
        always {
            // Post-build actions
        }
    }
}

    
    
    
 
    
                
