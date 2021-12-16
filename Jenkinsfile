pipeline {
          agent any 
          tools {
          //maven is tool as M2_HOME
          maven "M2_HOME"
          }
        stages{
        stage ('checkout'){ 
        steps {
        //clone the repositry from git 
        git 'https://github.com/NIKHIL9676/jenkins.git'
        }
        }
        stage ('build'){
        steps {
        //run maven build on unix agent
        sh "mvn -Dmaven.test.failure.ignore=true clean package"
         }
         }
		 }
		 }
