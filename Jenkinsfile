pipeline {

	agent any
    
stages {
        

	stage("Verification du version Maven") {
           steps {
                sh "mvn -version"
              
            }

        }
	
       stage("Supprimer le contenu du dossier target") {
            steps {
                script {
                    //this step attempts to clean the files and directories generated by Maven during its build
                    sh "mvn clean"
		  }
            }
        }
