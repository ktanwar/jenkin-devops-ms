pipeline {
	agent any
	stages{
		stage('Build'){
			steps{
				echo 'Build stage'
			}
		}
		stage('Test'){
			steps{
				echo 'Build Test'
			}
		}
	} post{
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
