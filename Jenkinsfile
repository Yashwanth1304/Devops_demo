pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Update Jira') {
            steps {
                jiraComment issueKey: 'DIP-2', body: "Build completed for commit ${env.GIT_COMMIT}"
            }
        }
    }
}

