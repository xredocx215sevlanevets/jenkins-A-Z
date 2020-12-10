pipeline {
   agent any

   stages {
      stage('checkout scm') {
         steps {
            script {
               sh 'git name-rev --name-only HEAD > GIT_BRANCH'
               git_branch = readFile('GIT_BRANCH').trim()
               
               env.GIT_BRANCH = git_branch.toLowerCase()
               env.IMAGE_NAME = git_branch.toLowerCase()
               env.CONTAINER_NAME = git_branch.toLowerCase()
            }
         }
      }

   }
}
