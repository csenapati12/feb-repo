node(){
        stage('clone the code'){
            checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/csenapati12/java-tomcat-maven-example.git']]]
        echo "clone"
        }
        stage('Build'){
            bat label: '', script: 'mvn package'
        echo "build"
            
        }
       stage('Unit test'){
       echo "Unit test"
       }
      stage('sonar analysis'){
       echo "Sonar analysis"
         } 
           stage('Nexus Upload'){
       echo "Nexus Upload"
         } 
        
    
}
