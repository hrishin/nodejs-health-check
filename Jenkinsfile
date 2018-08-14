#!/usr/bin/groovy

@Library('github.com/hrishin/fabric8-pipeline-library@nodejs')

def utils = new io.fabric8.Utils()
def envStage = utils.environmentNamespace('stage')
def envProd = utils.environmentNamespace('run')
def templateConfig = [:]
templateConfig["RELEASE_VERSION"] = "1.0.${env.BUILD_NUMBER}"

nodejsNode {
  templateConfig = templateConfig

  cd {
    echo "hello in cd"
  }
}
