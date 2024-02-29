// Scripted pipeline
// node {
// 	stage('Build') {
// 		echo "Build"
// 	}
// 	stage('Test') {
// 		echo "Test"
// 	}
// 	stage('Integration Test'){
// 		echo "Integration Test"
// 	}
// }

//Declarative pipeline

pipeline{
	agent any
	// agent {docker {image 'maven:3.6.3'}}
	// agent {docker {image 'node:13.8'}}
	environment{
    dockerHome= tool 'myDocker'
	mavenHome=tool 'myMaven'
	PATH="$dockerHome/bin:$mavenHome/bin:$PATH"
	}
	stages{
		stage('Build'){
			steps{
				echo "Build"
				echo "PATH-$PATH"
				echo "BUILD_NUMBER- $env.BUILD_NUMBER"
				 echo "BUILD_URL -$env.BUILD_URL "
			}
		}

		stage('Test'){
			steps{
				echo "test"
			}
		}

		stage('Integration Test'){
			steps{
				echo "Integration Test" 
			}
		}
	}
}