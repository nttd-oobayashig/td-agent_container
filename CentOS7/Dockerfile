FROM centos:7

RUN curl -L https://toolbelt.treasuredata.com/sh/install-redhat-td-agent3.sh | sh

EXPOSE 24224

CMD [ "sh", "-c", "td-agent", "-c", "$FLUENTD_CONF" ]
