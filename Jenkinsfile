node {

   stage('SCM') {
      // git clone
	  git 'https://github.com/YeshwanthReddyChalla/game-of-life.git'
   }
   
   stage ('build the packages') {
      // mvn package
	  sh 'mvn package'
   }

   stage ('archival') {
     // archiving artifacts
	 archiveArtifacts artifacts: 'gameoflife-core//target/*.jar'
   }

}

