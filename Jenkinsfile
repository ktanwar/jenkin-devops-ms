pipeline {
	agent any
	//agent { docker {image 'maven:3.6.3'}}
	environment{
		mavenHome = tool 'myMaven'
		PATH = '$PATH' + '$mavenHome/bin'
	}
	stages{
		stage('Build'){
			steps{
				echo 'stage Build'
				sh 'mvn --version'
				sh 'docker version'
				echo 'PATH - $PATH'
			}
		}
		stage('Test'){
			steps{
				echo 'stage Test'
			}
		}
	} 
	post{
		always{echo 'always'}
		success{echo 'success'}
		failure{echo 'failure'}
		changed{echo 'changed'}
	}
	
}
