node{
     
      stage('SCM Checkout'){
         git 'https://github.com/Abinaya2802/jenkins-maven-pipeline.git'
      }
      stage('Build'){
         // Get maven home path and build
         def mvnHome =  tool name: 'Maven 3.5.4', type: 'maven' 
         sh "'${mvnHome}/bin/mvn' -Dmaven.test.failure.ignore clean package"
      }       
}
