pipeline {
	    agent {
	        docker {
	            image 'httpd:2.4' // Use the same base image as in yur Dckerfile
	            args '-p 8081:80' // Expse prt 80 as 8080 n the hst
	        }
	    }
	    stages {
	        stage('Build') {
	            steps {
	                git 'https://github.com/PranadaT/php-project.git'
	                echo "Building the Docker image..."
	                //  N need t build, we are using the pre-built image.
	                docker.build("my-web-app-image", ".")
	            }
	        }
	        stage('Deploy') {
	            steps {
	                ech "Running the Docker container..."
}
}
}
}
