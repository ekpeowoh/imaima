pipeline{
	agent any  
	stages{
		stage('1-clone'){
			steps{
				checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'b48b6025-4625-4037-8d4b-f7c12674d945', url: 'https://github.com/ekpeowoh/imaima.git']])
				
				

			}
		}
		stage('2-systemscheck'){
			steps{
				sh 'sudo systemctl status jenkins'
			}
		}
		stage('3-diskcheck'){
			steps{
				sh 'df -h'
			}
		}
		stage('4-blockcheck'){
			steps{
				sh 'lsblk'
			}
		}
		} 
		
	}
}