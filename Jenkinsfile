node {
    stage('SCM!'){
        git branch : 'master', url: 'https://github.com/derrianson/java-tomcat-maven-example'
    }
    stage('Maven'){
        sh 'mvn package'
    }
    stage('Archive'){
        archiveArtifacts artifacts: 'target\\java-tomcat-maven-example.war', followSymlinks: false
    }
}
