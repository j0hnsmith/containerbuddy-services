FROM rabbitmq:3.6-management

# add containerbuddy and all our configuration
COPY opt/containerbuddy /opt/containerbuddy/

ENTRYPOINT ["/opt/containerbuddy/containerbuddy", "-config", "file:///opt/containerbuddy/rabbitmq.json", "/docker-entrypoint.sh"]
CMD ["rabbitmq-server"]
