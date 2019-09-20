node{
    checkout scm
    stage("run security scan"){
      sh "docker run --network=bundlev2_prodnetwork --rm -t owasp/zap2docker-stable zap-baseline.py -t http://tomcat:10000/"
    }
}
