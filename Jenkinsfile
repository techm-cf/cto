node {
   withEnv(["PATH+MAVEN=${tool 'apache-maven-3.5.3'}bin"]) {
   stage('Preparation') {
        checkout scm
           checkout scm

        }
   stage('Build') {
        mvnHome = tool 'apache-maven-3.5.3'
               sh 'mvn -f controllers-unittest/pom.xml clean install'
   }
    stage('Sonar Code analysis') {
            withSonarQubeEnv('sonar') {
                sh 'mvn -f controllers-unittest/pom.xml clean package sonar:sonar'
            }
    stage('Record Artifacts on  Nexus') {
     sh 'curl -v --user admin:admin123 --upload-file /var/lib/jenkins/workspace/techm-cf_New_Repo10_master-35L3B3FZRMVEQQCJEQRDWGG6Y4BYWCBAECXZZUB5CK5LIHQPYKUQ/control$

   }
       stage('Push app to CF') {
                pushToCloudFoundry cloudSpace: 'dev', credentialsId: 'b7c24062-6ea4-4876-89a1-96b3c2b430b2', manifestChoice: [manifestFile: '/var/lib/jenkins/workspace$

    }
}
}
}
