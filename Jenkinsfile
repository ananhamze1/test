pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('aaa') {
      steps {
        script {
          STAGE1="<b><font color=red>--</font></b>"
        }

        script {
          final job1Result = build ('blue/BlueOcean')
          STAGE1=${jobresult.number}
        }

      }
    }

    stage('egfde') {
      steps {
        sh 'echo $STAGE1'
      }
    }

  }
}