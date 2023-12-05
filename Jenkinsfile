//podTemplate(containers: [
//    containerTemplate(name: 'maven', image: 'maven:3.8.1-jdk-8', command: 'sleep', args: '99d'),
//    containerTemplate(name: 'golang', image: 'golang:1.16.5', command: 'sleep', args: '99d')
//  ]) {

    node('jenkins') {
        
        stage('Get a Maven project') {
            git 'https://github.com/jenkinsci/kubernetes-plugin.git'
            container('jenkins-worker') {
                stage('Build a Maven project') {
                    sh 'mvn -B -ntp clean install'
                }
            }
        }
    }
