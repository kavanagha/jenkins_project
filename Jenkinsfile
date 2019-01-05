pipeline {
  agent any
  stages {
    stage('Build'){
      steps {
		bat "javac 'C:\\Users\\ailis\\Documents\\College\\Fourth Year\\Software Engineering\\studentAttendance\\Student.java'"
        bat "javac -cp .; 'C:\\Program Files\\junit4.10\\junit-4.10.jar' 'C:\\Users\\ailis\\Documents\\College\\Fourth Year\\Software Engineering\\studentAttendance\\studentTest.java'"
      }
    }
    stage('Test') {
      steps { 
        bat "java -cp .;'C:\\Program Files\\junit4.10\\junit-4.10.jar' org.junit.runner.JUnitCore 'C:\\Users\\ailis\\Documents\\College\\Fourth Year\\Software Engineering\\studentAttendance\\studentTest'" 
      }
    }
  }
}