pipeline {
    agent { label 'slave2' }

    stages {
        stage('Stage 1') {
            steps {
                echo "Done at worker2"
            }
        }
    }
    agent { label 'slave1' }

    stages {
        stage('Stage 2') {
            steps {
                echo "Done at worker1"
            }
        }
    }
}
