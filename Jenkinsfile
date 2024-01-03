pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=addingsonnartoproject -Dsonar.organization=addingsonnartoproject -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=2d7ffb96e8ed374303a10c59630c288e67f5663b'
			}
        } 
  }
}
