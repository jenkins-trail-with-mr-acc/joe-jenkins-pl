pipeline {
    agent any
    stages {
        stage('first_stage') {
            steps {
            script {
            try {
                sh "touch /tmp/test1"
            } catch (Exception e) {
            status = -1
            }
            }
            }
        }
        stage('second_stage') {
            steps {
            echo "creating secound file"
            script {
            try {
                sh "touch tmp/test2"
            } catch (Exception e) {
            status = -1
            }
            }
            }
        }
        
        
    }  
}
