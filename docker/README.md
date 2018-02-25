## Manual tweaks:

* Change the jenkins home directory permissions and owner (so jenkins can freely write there and we don't need sudo):
    - `$ chmod -R 777 /var/lib/docker/volumes/jenkins-data`
    - `$ chown -R 1000:1000 /var/lib/docker/volumes/jenkins-data`
