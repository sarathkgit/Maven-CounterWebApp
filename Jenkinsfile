node{
    
    def mvnHome = tool name: 'maven-3', type: 'maven'
    
    stage('SCM Checkout'){
         git 'https://github.com/sarathkgit/Maven-CounterWebApp'
    }
    
    stage('Compile Package'){
         
         sh "${mvnHome}/bin/mvn package"
    }
    
    stage('Email Notification'){
        
        mail bcc: '', body: '''Hi
        This is Jenkins Job Notification

        Thanks and Regards,
        Sarath''', cc: '', from: '', replyTo: '', subject: 'Jenkins Mail Notification Job', to: 'sarath0969@gmail.com'
     }
}
