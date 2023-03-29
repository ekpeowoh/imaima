pipeline{
    agent any
    stages{
        stage('1-clonecode'){
            steps{
                sh 'df -h'
            }
        }
        stage('2-memorycheck'){
            steps{
                sh 'free -g'
            }
        }
        stage('3-welcomepage'){
            steps{
                echo "welcome to jenkins"
            }
        }
    }
}