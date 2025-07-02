pipeline {
       agent any
	   stages {
	          stage("build") {
			        steps {
					       git branch: 'main', url: 'https://github.com/Bushra112004/Jenkins.git'
						   }
						}
			  stage("testing") {
			        steps {
					       sh 'sudo mvn clean package'
						   }
						}
			  stage("execute") {
			        steps {
					       sh 'sudo java -jar target/*.jar > /var/lib/jenkins/workspace/maven/text.txt'

						   }
						}
		}	
}
