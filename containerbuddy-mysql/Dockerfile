FROM mysql:5.6

# add containerbuddy and all our configuration
COPY opt/containerbuddy /opt/containerbuddy/

ENTRYPOINT ["/opt/containerbuddy/containerbuddy", "-config", "file:///opt/containerbuddy/mysql.json", "/entrypoint.sh"]
CMD ["mysqld"]
