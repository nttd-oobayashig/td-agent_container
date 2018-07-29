td-agent container
====

Overview

## Description
Dockerfile collection for verification of td-agent.

## Demo
docker run -d -p 24224:24224/tcp -p 24224:24224/udp -v /tmp/container1/log:/log -v /opt/container1/conf:/td-agent/container1/conf -e FLUENTD_CONF=/td-agent/container1/conf/td-agent.conf --name td-agent1 td-agent

