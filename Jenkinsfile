pipeline
{

//running on the slave label
agent {label 'slave'};

stages{
	stage('Clone And Build Project'){
		steps{
			//cloning the project PetClinic			 
sh "git clone https://github.com/spring-projects/spring-petclinic.git"

sh "pwd"
dir('spring-petclinic'){
sh "pwd"
}
			
			//building the application
			script{
				"./mvnw package"
			      }
		     }
					}
      }
}
