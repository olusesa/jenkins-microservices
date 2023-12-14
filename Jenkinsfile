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
	//agent any
	agent {docker { image 'maven:3.8.6'}}
	//agent {docker { image 'node:13.8'}}
	stages {
		stage('Build') {
			steps{
			echo "Build"
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

