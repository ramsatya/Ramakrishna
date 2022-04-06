node{
      
     
    stage('git-clone'){
        git  branch: 'development', credentialsId: 'github', url: 'https://github.com/ramsatya/Ramakrishna.git'
    }
    
    stage('maven-build')
     def mavenHome =  tool name: "maven-3.6.3", type: "maven"
      def mavenCMD = "${mavenHome}/bin/mvn"
      sh "${mavenCMD} clean package"
      
    }

