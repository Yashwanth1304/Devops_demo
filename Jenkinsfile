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
                jiraComment issueKey: 'PROJ-123', body: "Build completed for commit ${env.GIT_COMMIT}"
            }
        }
    }
}

