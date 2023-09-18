pipeline {
    agent any
    tools { 
        maven 'Maven_3_6_3'  
    }
    stages{
        stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=my-first-org-shiv-b1 -Dsonar.organization=my-first-org-shiv-b1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=cbebe62a30ac79ee509bc6e071e09b9dfa42a53f'
	    }
        } 
    }
}
