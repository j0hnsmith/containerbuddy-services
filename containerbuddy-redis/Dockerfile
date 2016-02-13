FROM redis:3.0.5

# add containerbuddy and all our configuration
COPY opt/containerbuddy /opt/containerbuddy/

ENTRYPOINT ["/opt/containerbuddy/containerbuddy", "-config", "file:///opt/containerbuddy/redis.json", "/entrypoint.sh"]
CMD ["redis-server"]
