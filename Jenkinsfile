node{
    stage("run security scan"){
      sh "sudo docker run --network=bundlev2_prodnetwork --rm -t owasp/zap2docker-stable zap-baseline.py -t http://tomcat:10000/"
      sh "exit 0"  
    }
}
