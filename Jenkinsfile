pipeline {
    agent label {'build_on_slave'}
    stages {
        stage('Git-checkout') {
            steps {
                echo "Checking out code from Git repository";
                git 'https://github.com/rahulkhullar/myFirstWebApplication'
            }
        }
    
    stage('Build') {
        steps {
            echo "Building the checkout project";
            sh 'mvn package'
        }
    }
    
    stage('Unit-test') {
        steps {
            echo "Running Junit tests";
        }
    }
    
    stage('Quality-Gate') {
        steps {
            echo "verifying quality gates";
            
        }
    }
    
    stage('Deploy') {
        steps {
            echo "Deploying to stage environments for more tests cases";
        }
    }
}

    post {
        always {
            echo "This will always run!!"
        }
        success {
            echo "This will run only if successful"
        }
        failure {
            echo "This will run only if failed"
        }
        unstable {
            echo "This will only run if the run was marked as unstable"
        }
        changed {
            echo "This will only change if the state of pipeline is changed from failling to successful"
        }
    
}
}


