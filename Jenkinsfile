pipeline {
  agent any
  tools { 
        maven 'maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sonarcloud-buggy -Dsonar.organization=sonarcloud-buggy -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=f66702d874ec3aff9df40586f894cc84b6f0a720'
			}
        } 
  }
}
