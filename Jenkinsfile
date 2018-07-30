pipeline{
	agent any
	
	stages {
		stage ('Compile Stage') {
	
			steps{
				withMaven(maven : 'Maven 3.1.1'){
				bat 'mvn compile'
				}
		    }
		}
		stage ('Testing Stage') {
	
			steps {
				withMaven(maven : 'Maven 3.1.1'){
				bat 'mvn test'
				}
		    }
		}
		stage ('Deployment Stage') {
	
			steps{
				withMaven(maven : 'Maven 3.1.1'){
				bat 'mvn deploy'
				}
		    }
		}	   	   
   }	
}