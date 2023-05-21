pipeline{
	agent any
	tools{
	    maven 'maven_3_5_0'
	}
	stages{
	    stage('Build Maven'){
	        steps{
	            sh 'mvn clean install'
	        }
	    }
	    stage('Build docker image'){
	        steps{
	            script{
	                sh 'docker build -t '
	            }
	        }
	    }
	    stage('Push docker Image to hub')
	        steps{
	            script{
	                sh 'docker login -u <hub_name> -p $(pwd variable)'
	                sh 'docker push <docker-hub_name>/<image_name>'
	            }
	        }
	}   
}
