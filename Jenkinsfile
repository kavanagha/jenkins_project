pipeline {
  agent any
  stages {
	stage ('Fetch'){
		steps{
			bat "git fetch origin"
		}
	}
    stage('Build'){
      steps {
	    bat "javac -version"
		bat "javac Student.java"
        bat 'javac -cp .;"C:\\Program Files\\junit4.10\\junit-4.10.jar" studentTest.java'
      }
    }
    stage('Test') {
      steps { 
        bat 'java -cp .;"C:\\Program Files\\junit4.10\\junit-4.10.jar" org.junit.runner.JUnitCore studentTest' 
      }
    }
  }
}