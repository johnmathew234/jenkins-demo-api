pipeline
	{
	agent any
	stages {
	
		stage('Build Application'){
		steps{
		bat 'mvn clean install -DskipTests'
		}
		}
		
		
		
		stage('Munit Tests'){
		steps{
		bat 'mvn clean test'
		}
		}
		
		
		stage('Deploy Application to CloudHub'){
		steps{
		bat 'mvn package deploy -Danypoint.username=jmp22041112 -Danypoint.password=John00000 -DapplicationName=jenkins-demo-api -DmuleDeploy'
		}
		}
		
		
	}
	}