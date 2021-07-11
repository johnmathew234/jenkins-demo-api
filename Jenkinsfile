pipeline
	{
	agent any
	stages {
	
		stage('Build Application'){
		steps{
		sh 'mvn clean install -DskipTests'
		}
		}
		
		
		
		stage('Munit Tests'){
		steps{
		sh 'mvn clean test'
		}
		}
		
		
		stage('Deploy Application to CloudHub'){
		steps{
		sh 'mvn package deploy -Danypoint.username=jmp22041112 -Danypoint.password=John00000 -DapplicationName=jenkins-demo-api -DmuleDeploy'
		}
		}
		
		
	}
	}
