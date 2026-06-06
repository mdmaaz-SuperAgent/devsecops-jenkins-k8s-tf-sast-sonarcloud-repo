pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=secguru123 -Dsonar.organization=secguru123 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=958058fac36d22a25096e9ae5a285c04298bdcdf'
			}
        } 
  }
}
