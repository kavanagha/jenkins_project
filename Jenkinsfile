pipeline {
  agent any
  stages {
    stage('Build'){
      steps {
		sh "javac Student.java"
        sh "javac -cp .;'C:\\Program Files\\junit4.10\\junit-4.10.jar' studentTest.java"
      }
    }
    stage('Test') {
      steps { 
        sh "java -cp .;'C:\\Program Files\\junit4.10\\junit-4.10.jar' org.junit.runner.JUnitCore studentTest" 
      }
    }
  }
}