# prometheus-monitoring

curl -k --cert ./od-elastic/certs/admin.pem --key ./od-elastic/certs/admin-key.pem  https://localhost:9200/

chmod +x ./plugins/opendistro_security/tools/securityadmin.sh

./plugins/opendistro_security/tools/securityadmin.sh -cd /usr/share/elasticsearch/plugins/opendistro_security/securityconfig/ -icl -nhnv -cacert /usr/share/elasticsearch/config/certs/root-ca.pem -cert /usr/share/elasticsearch/config/certs/admin.pem -key /usr/share/elasticsearch/config/certs/admin-key.pem