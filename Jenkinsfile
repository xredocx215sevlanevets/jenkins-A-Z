pipeline {
   // agent none

   // agent {
   //    label: "Slave 1"
   // }

   agent {
      node {
         label 'Slave 1'
         customWorkspace '/home/ec2-user/customWorkspace'
      }
   }

   stages {
      stage('checkout scm') {
         steps {
            echo 'Hello World'
         }
      }
   }
}
