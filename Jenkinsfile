pipeline {
    agent any
    stages {
        stage('LoadJenkinsfile') {
            steps {
               
              def workspace = pwd()
               println "current workspace : ${workspace}"
              new File(workspace+"/projects/Veridic_NewJersey").list().each {
               if( it.contains("Jenkinsfile")){
                    def jFilepath = workspace+"/projects/Veridic_NewJersey/" + it;
                    println jFilepath
            
                    def jFile = load jFilepath
                    jFile.start()
        }
     }     

                               
            }
        }
    }
}
