// node {
// 	stage('Build') {
// 		echo "Build"
// 	}
// 	stage('Test') {
// 		echo "Test"
// 	}
// 	stage('Functional Test') {
// 		echo "Functional Test Completed Succefully"
// 	}
// 	stage('QADeploy') {
// 		echo "Deployment to QA Completed Succefully"
// 	}
// 	stage('Staging Deploy') {
// 		echo "Deployment to Staging Completed Succefully"
// 	}
// }

pipeline {
	agent any
	// agent {docker {image 'maven:3.6.3'}}
	//agent {docker {image 'node:13.8'}}
	environment {
		mavenHome = tool 'wyzlabmaven'
		dockerHome = tool 'wyzlabdocker'
		PATH = "$mavenHome/bin:$dockerHome/bin:$PATH"
	}
	stages {
		stage('Build') {
			steps{
			sh 'mvn --version'
			sh 'docker version'
			echo "Build"
			echo "PATH - $PATH"
			echo "BUILD_NUMBER - $env.BUILD_NUMBER"
			echo "BUILD_ID - $env.BUILD_ID"
			echo "JOB_NAME - $env.JOB_NAME"
			echo "BUILD_TAG - $env.BUILD_TAG"
			echo "BUILD_URL - $env.BUILD_URL"

			}
		}
		stage('Test') {
			steps{
			echo "Test"
		}
		}
		stage('Functional Test') {
			steps{
			echo "Functional Test Completed Succefully"
		}
		}
		stage('QADeploy') {
			steps{
			echo "Deployment to QA Completed Succefully"
		}
		}
		stage('Staging Deploy') {
			steps{
			echo "Deployment to Staging Completed Succefully"

		}
		}
	}
}

