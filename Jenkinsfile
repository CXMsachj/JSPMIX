pipeline {
	agent any
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/sachin/Documents/Jenkins/apache-maven-3.8.6-bin/apache-maven-3.8.6/bin/mvn install'
	                 }}
		stage('Deployment'){
		    steps {
			
			sh 'cp target/JSPMIX.war /home/sachin/Documents/Jenkins/apache-tomcat-9.0.70/webapps'
	}
}}}
