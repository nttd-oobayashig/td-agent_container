FROM amazonlinux:2018.03

RUN curl -L https://toolbelt.treasuredata.com/sh/install-amazon2-td-agent3.sh | sh

EXPOSE 24224

CMD [ "sh", "-c", "td-agent", "-c", "$FLUENTD_CONF" ]
