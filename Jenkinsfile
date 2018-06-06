pipeline {
  agent any
  stages {
	stage('maven clean'){
	  steps {
		withMaven(maven: 'M2_Home') {
		  sh 'mvn clean'
		}
	  }
	}		
   
    stage('maven complie'){
	  steps {
		withMaven(maven: 'M2_Home') {
		  sh 'mvn compile'
		}
	  }
	}
	
	stage('maven clean'){
	  steps {
		withMaven(maven: 'M2_Home') {
		  sh 'mvn package'
		}
	  }
	}					
  }   
}