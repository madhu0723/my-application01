node{
   stage('SCM Checkout'){
     git 'https://github.com/madhu0723/my-application01'
      
   }
   stage('Build'){
      def mvnHome = tool name: 'm2', type: 'maven'
      sh  "${mvnHome}/bin/mvn clean package"
   }
   
     
}
