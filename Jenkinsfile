pipeline {
  agent any
  tools { 
       maven 'Maven-3.8.4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=gntek323-maker_devsecops-jenkins-k8s-tf-sast-sonarcloud-repo -Dsonar.organization=gntek323-maker -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=57b2f1e9bf6240d1f36a7d1ea1c4c20d47741bdb'

			}
        } 
  }
}
