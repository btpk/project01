node{

stage('scm'){
//git clone

  git 'https://github.com/spring-projects/spring-petclinic.git'
}
 stage('build the package'){
     //mvn package
	 
	 sh 'mvn package'
	 
	 }
	 stage('archival'){
	  //targets/*.jar
	   
	  archive 'target/*.jar'
	  
	  }
	  stage ('test results'){
	  
	  junit 'target/surefire-reports/*.xml'
	  
	  }
}