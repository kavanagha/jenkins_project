pipeline {
  agent any
  stages {
    stage('Build'){
      steps {
	    bat "set 'path=%path%;C:\\Program Files\\Java\\jdk1.8.0_121\\bin'"
		bat "echo %path%"
		bat "javac Student.java"
        bat "javac -cp .; 'C:\\Program Files\\junit4.10\\junit-4.10.jar' studentTest.java"
      }
    }
    stage('Test') {
      steps { 
        bat "java -cp .;'C:\\Program Files\\junit4.10\\junit-4.10.jar' org.junit.runner.JUnitCore studentTest" 
      }
    }
  }
}