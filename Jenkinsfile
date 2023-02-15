pipeline { 
   agent any

    stages {
        stage('Git Pull') {
            steps {
                // Get code from a GitHub repository
                // Make sure to add your own git url and credentialsId
				git url: 'https://github.com/KARISHMA21/jenkins.git',
				branch: 'main',
//                 credentialsId: 'GitCredential'
            }
        }
        stage('Maven Build') {
            steps {
                // Maven build, 'sh' specifies it is a shell command
                sh 'mvn clean install'
            }
        }
     stage('Test Code') {
            steps {
                 echo "Inside Test code stage "
            }
        }
        
        stage('Deliver Code') {
            steps {
                 echo "Inside Deliver code stage"
            }
        }
        
        stage('Deploy Code') {
            steps {
                 echo "Inside Deploy code stage"
            }
        }
    } 
}
