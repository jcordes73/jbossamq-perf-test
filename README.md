# JBoss A-MQ perf test

mvn activemq-perf:consumer -DsysTest.propsConfigFile=src/main/resources/perf-test-nonpersistent-nontransacted.properties -Dfactory.brokerURL=nio://localhost:61616 -DsysTest.numClients=10
mvn activemq-perf:producer -DsysTest.propsConfigFile=src/main/resources/perf-test-nonpersistent-nontransacted.properties -Dfactory.brokerURL=nio://localhost:61616 -DsysTest.numClients=10 -Dproducer.messageSize=1024

