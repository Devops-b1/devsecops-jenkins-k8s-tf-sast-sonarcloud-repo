pipeline {
    agent any
    tools { 
        maven 'Maven_3_6_3'  
    }
    stages {
        stage ('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=shiv-roshan-dev-project-b1 -Dsonar.organization=my-shiv-roshan-dev-project-b1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=ceb44d2722d04eac210442b87f0622515be47367'
	    }
        } 
    }
}
