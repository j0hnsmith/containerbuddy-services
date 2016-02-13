FROM postgres:9.4.4

# add containerbuddy and all our configuration
COPY opt/containerbuddy /opt/containerbuddy/

ENTRYPOINT ["/opt/containerbuddy/containerbuddy", "-config", "file:///opt/containerbuddy/postgres.json", "/docker-entrypoint.sh"]
CMD ["postgres"]
