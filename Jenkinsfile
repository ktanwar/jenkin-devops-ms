pipeline {
	agent any
	//agent { docker {image 'maven:3.6.3'}}
	stages{
		stage('Build'){
			steps{
				echo 'stage Build'
			}
		}
		stage('Test'){
			steps{
				echo 'stage Test'
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
