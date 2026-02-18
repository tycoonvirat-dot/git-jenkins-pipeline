pipeline{
 tools{
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }
     agent any
	  
	  stages{
	  
	  stage("checkout"){
	   steps{
	   git 'https://github.com/tycoonvirat-dot/git-jenkins-pipeline.git'
	   }
	                  }
	
	   stage("compile"){
	    steps{
		 sh 'mvn compile'
		}
		}
	   stage("test"){
	    steps{
		 sh 'mvn test'
		}
		}
	  stage("package"){
	    steps{
		 sh 'mvn package'
		}
		}
	  }
	}
