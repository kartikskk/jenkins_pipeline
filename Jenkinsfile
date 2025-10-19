pipeline {
    agent none // no global agent, since each stage defines its own

    stages {
        stage('Stage 1') {
            agent { label 'slave2' }
            steps {
                echo "Done at worker2"
            }
        }

        stage('Stage 2') {
            agent { label 'slave1' }
            steps {
                echo "Done at worker1"
            }
        }
    }
}
