node {
        stage('Checkout') {
            git url: 'https://github.com/Vijji456/ProjectWeek2_Products.git',  branch: 'master'
            echo '****************CHECKOUT SUCCESSFUL****************'
        }
       

       
			
	stage('Build') {
		def mvn_version = 'MAVEN_HOME'
		withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"]) {
			sh 'mvn site'
			}
		}
}
