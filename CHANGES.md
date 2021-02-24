Changes by Version
==================
Release Notes.

8.5.0
------------------
#### Project
* Update frontend-maven-plugin to 1.11.0, for Download node x64 binary on Apple Silicon.
* Add E2E test for VM monitoring that metrics from Prometheus node-exporter.

#### Java Agent
* Remove invalid mysql configuration in agent.config.
* Add net.bytebuddy.agent.builder.AgentBuilder.RedefinitionStrategy.Listener to show detail message when redefine errors occur.
* Fix ClassCastException of log4j gRPC reporter.
* Fix NPE when Kafka reporter activated.
* Enhance gRPC log appender to allow layout pattern.
* Fix apm-dubbo-2.7.x-plugin memory leak due to some Dubbo RpcExceptions.

#### OAP-Backend
<<<<<<< HEAD
* Make meter receiver support MAL.
* Support influxDB connection response format option. Fix some error when use JSON as influxDB response format.
* Support Kafka MirrorMaker 2.0 to replicate topics between Kafka clusters.
* Add the rule name field to alarm record storage entity as a part of ID, to support multiple alarm rules triggered for one entity. The scope id has been removed from the ID.
* Fix MAL concurrent execution issues.
* Fix group name can't be queried in the GraphQL.
* Fix potential gRPC connection leak(not closed) for the channels among OAP instances.
* Filter OAP instances(unassigned in booting stage) of the empty IP in KubernetesCoordinator.
* Add component ID for Python aiohttp plugin requester and server.
* Fix H2 in-memory database table missing issues
* Add component ID for Python pyramid plugin server.
* Add component ID for NodeJS Axios plugin.
* Fix searchService method error in storage-influxdb-plugin.
* Add JavaScript component ID.
* Fix CVE of UninstrumentedGateways in Dynamic Configuration activation.
* Improve query performance in storage-influxdb-plugin.
* Fix the uuid field in GRPCConfigWatcherRegister is not updated.
* Support Envoy {AccessLog,Metrics}Service API V3.
* Adopt the [MAL](docs/en/concepts-and-designs/mal.md) in Envoy metrics service analyzer.
* Fix the priority setting doesn't work of the ALS analyzers.
* Fix bug that `endpoint-name-grouping.yml` is not customizable in Dockerized case.
* Adding the JVMMemoryPool usage ratio metric for the convenience of tuning JVM Memory for Large-scale Services and analyzing memory leak problems.
=======
* Allow user-defined `JAVA_OPTS` in the startup script.
* Metrics combination API supports abandoning results.
* Add a new concept "Event" and its implementations to collect events.
* Add some defensive codes for NPE and bump up Kubernetes client version to expose exception stack trace.
* Update the `timestamp` field type for `LogQuery`.
* Support Zabbix protocol to receive agent metrics.
* Update the Apdex metric combine calculator.
* Enhance `MeterSystem` to allow creating metrics with same `metricName` / `function` / `scope`.
* Storage plugin supports postgresql.
* Fix kubernetes.client.opeanapi.ApiException.
* Remove filename suffix in the meter active file config.
* Introduce log analysis language (LAL).
>>>>>>> 665a07cb0f97316c6c98425d1a0fcf363214483e

#### UI
* Update selector scroller to show in all pages.
* Implement searching logs with date.

#### Documentation


All issues and pull requests are [here](https://github.com/apache/skywalking/milestone/76?closed=1)

------------------
Find change logs of all versions [here](changes).
