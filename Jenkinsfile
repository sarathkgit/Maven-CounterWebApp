node{
    
    def mvnHome = tool name: 'maven-3', type: 'maven'
    
    stage('SCM Checkout'){
         git 'https://github.com/sarathkgit/Maven-CounterWebApp'
    }
    
    stage('Compile Package'){
         
         sh "${mvnHome}/bin/mvn package"
    }
}
