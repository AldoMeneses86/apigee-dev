export path=sa-apigee-deployer.json
mvn install -Ptest -Dorg=apigee-svc-eval-01 -Denv=eval -Dfile=$path

mvn clean install -Ptest -Dorg=apigee-svc-eval-01  -Denv=eval -Dbearer=$(gcloud auth print-access-token)