pipeline {
  agent {
    docker {
      image 'ubuntu:18.04'
      args '-p 22:22'
    }

  }
  stages {
    stage('docker pull') {
      steps {
        sh '''apt-get -y install gcc g++ gdb  autoconf libtool make cmake;
apt-get -y install ssh ntp vim wget  telnet;
apt-get -y install git net-tools inetutils-ping;'''
      }
    }

  }
  environment {
    LANG = 'en_US.UTF-8'
  }
}