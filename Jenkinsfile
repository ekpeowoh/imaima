pipeline{
	agent any  
	stages{
		stage('1-clone'){
			steps{
				sh 'lscpu'
			}
		}
		stage('2-systemscheck'){
			steps{
				sh 'sudo systemctl status jenkins'
			}
		}
	}