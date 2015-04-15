curl --data-binary @job-server-tests/target/job-server-tests-0.4.1.jar localhost:8090/jars/test
curl -d "input.string = a b c a b see" 'localhost:8090/jobs?appName=test&classPath=spark.jobserver.WordCountExample'
curl localhost:8090/jobs/5453779a-f004-45fc-a11d-a39dae0f9bf4