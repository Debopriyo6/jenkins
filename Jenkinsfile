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
				echo "Test"
			}
		}

		stage('Integration Test'){
			steps{
				echo "Integration Test" 
			}
		}
	}
}