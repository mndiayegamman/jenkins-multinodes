//podTemplate {
//    node('jenkins-slave') {
//        stage('Get a Maven project') {
//            git 'https://github.com/jenkinsci/kubernetes-plugin.git'
//            container('jenkins-worker') {
//                stage('Build a Maven project') {
//                    sh 'mvn -B -ntp clean install'
//                }
//            }
//        }
//    }
//}
podTemplate {
    node('jenkins-slave') {
        stage('Run shell') {
            sh 'echo hello world'
        }
    }
}
