pipeline
	{
	agent any
	stages {
	
		stage('Build Application'){
		steps{
		bat 'sh clean install -DskipTests'
		}
		}
		
		
		
		stage('Munit Tests'){
		steps{
		bat 'sh clean test'
		}
		}
		
		
		stage('Deploy Application to CloudHub'){
		steps{
		bat 'sh package deploy -Danypoint.username=jmp22041112 -Danypoint.password=John00000 -DapplicationName=jenkins-demo-api -DmuleDeploy'
		}
		}
		
		
	}
	}