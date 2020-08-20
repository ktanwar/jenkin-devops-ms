pipeline {
	agent { docker {image 'maven:3.6.3'}}
	stages{
		stage('Build'){
			steps{
				sh 'docker --version'
				echo 'stage'
			}
		}
		stage('Test'){
			steps{
				sh 'docker pull mysql'
				echo 'Test'
			}
		}
	} 
	post{
		always{
			echo 'always'
		}
		success{
			echo 'success'
		}
		failure{
			echo 'failure'
		}
		changed{
			echo 'changed'
		}
	}
	
}
