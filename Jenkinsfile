pipeline{
    agent{label 'linux'}

stages{
    stage('checkout'){
        steps{
            git'https://github.com/nizarnasraoui9/learning_jenkins.git'
        }
    }
    stage('Build'){
        steps{
            sh 'mvn clean compile'
        }
    }
    stage('Test'){
        steps{
            sh 'mvn test'
        }
    }
    stage('Package'){
        steps{
            sh 'mvn package'
        }
    }
}
