pipeline {
    agent any 
    tools {
        maven "Maven3"
    }
    stages {
        stage('Clone') { 
            steps {
                git 'https://github.com/PranjalPatil888/MyHelloWorld_springboot.git'
                sh 'echo "Git Repo cloned Successfull"'
            }
        }
        stage('Compile') { 
            steps {
                sh 'mvn compile'
            }
        }
        stage('Test') { 
            steps {
                sh 'mvn test'
            }
        }
        stage('Package') { 
            steps {
                sh 'mvn package'
            }
        }
        stage('Deploy') { 
            steps {
                sh 'echo "Deployement Successfull"'
            }
        }
    }
}
