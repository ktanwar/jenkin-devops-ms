pipeline {
	agent any
	stages{
		stage('Build'){
			steps{
				echo 'stage'
			}
		}
		stage('Test'){
			steps{
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
