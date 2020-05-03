node{
   stage('SCM Checkout'){
     git 'https://github.com/madhu0723/my-application01'
      
   }
   stage('Build'){
      def mvnHome = tool name: 'm2', type: 'maven'
      sh  "${mvnHome}/bin/mvn clean package"
   }
   
   stage('email-notificaiton'){
      
      mail bcc: '', body: '''Hi Team, 

      Thanks for Mail notifications.

      Regards,

      Madhusudhan M.''', 
      cc: 'madhum.java@gmail.com', from: '', replyTo: '', subject: 'My Notification Testing', to: 'madhumatt02@gmail.com'
      
   }
   
   
}
