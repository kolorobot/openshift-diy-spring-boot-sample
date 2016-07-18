#!/bin/bash

source $OPENSHIFT_CARTRIDGE_SDK_BASH

set -x

export JAVA_HOME=/etc/alternatives/java_sdk_1.8.0
export PATH=$JAVA_HOME/bin:$PATH

cd $OPENSHIFT_REPO_DIR
nohup java -Xms384m -Xmx412m -jar target/*.jar --server.port=${OPENSHIFT_DIY_PORT} --server.address=${OPENSHIFT_DIY_IP} --spring.profiles.active=openshift &
