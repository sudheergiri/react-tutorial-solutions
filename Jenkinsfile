pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                sh "sudo npm install"
                sh "sudo npm run build"
                sh "sudo npm start"
            }
     }      
     stage("Deploy") {
         steps {
              sh 'sudo cp -r ./* /home/ec2-user/react-tutorial-solutions/'
         }
     }
   }
}
