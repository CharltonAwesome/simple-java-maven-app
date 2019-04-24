pipeline {
    agent {
        docker {
		echo 'file file not text file'
            image 'maven:3.9-alpine' 
            args '-v /root/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}