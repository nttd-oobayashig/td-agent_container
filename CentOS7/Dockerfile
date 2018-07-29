FROM centos:7

RUN curl -L https://toolbelt.treasuredata.com/sh/install-redhat-td-agent3.sh | sh

RUN set -x && mkdir -p /opt/apps
COPY ../startup.sh /opt/apps/startup.sh
RUN set -x && chmod 755 /opt/apps/startup.sh

EXPOSE 24224

CMD ["/opt/apps/startup.sh"]
