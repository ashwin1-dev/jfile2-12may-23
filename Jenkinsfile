pipeline {
	agent any

     	tools {
		maven "jenkin-maven"
	    }

	stages {
		stage ("build") {
			steps {
				git 'https://github.com/ashwin1-dev/vlc1-11may23.git'
				sh "mvn  clean install"
				sh "scp /var/lib/jenkins/.m2/repository/com/tux/st1/vlc1/1.0-SNAPSHOT/vlc1-1.0-SNAPSHOT.jar   192.168.10.32:/opt/apache-tomcat-8.5.88/webapps
				}
			       }
          	}
}
