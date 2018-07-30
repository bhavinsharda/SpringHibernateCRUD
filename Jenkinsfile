pipeline{
	agent any
	
	stages {
		stage ('build') {
	
			steps{			
				bat 'mvn clean package'
		    }
		}
		
		stage ('Compile Stage') {
	
			steps{			
				bat 'mvn compile'
		    }
		}
		stage ('Testing Stage') {
	
			steps {			
				bat 'mvn test'
		    }
		}
		stage ('Deployment Stage') {
	
			steps{		
				bat 'mvn deploy:deploy'
		    }
		}	   	   
   }	
}
