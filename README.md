tar -czvf - api-0.0.1-SNAPSHOT.jar | split -b 20M - archive.tar.gz
cat archive.tar.* | tar -xzvf -
