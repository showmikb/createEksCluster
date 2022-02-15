
pipeline{

	agent any

	
	stages {

		

        stage('eks deploy') {

			steps {
			  sh 'eksctl create cluster -f eksworkshop.yaml'

			}
		}
	}

	post {
		always {

            		cleanWs()
			
            		echo "done"
		}
	}

}