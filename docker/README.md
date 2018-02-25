## Manual tweaks:

* Change the jenkins home directory permissions and owner (so jenkins can freely write there and we don't need sudo):
    - `$ chmod -R 777 /var/lib/docker/volumes/jenkins-data`
    - `$ chown -R 1000:1000 /var/lib/docker/volumes/jenkins-data`
<!-- * Change the npm packages folder permissions so npm doesn't complain when jenkins is installing packages:
    - `$ chmod -R 777 /usr/lib/node_modules`
 -->
