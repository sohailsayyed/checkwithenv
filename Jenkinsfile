pipeline{
    agent any
    triggers {
    github(
        events: [githubBranchCreated()],
        branches: [[pattern: 'release/*']],
        skipFirst: false
    )
}

    stages{
        stage("Show branch") {
            steps{
                script{
                    echo "${env.GIT_BRANCH}"
                    echo "${env.BRANCH_NAME}"
                }
            }
        }
    }
}
