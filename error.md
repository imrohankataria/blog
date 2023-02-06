Pulling zookeeper (debezium/zookeeper:latest)...
latest: Pulling from debezium/zookeeper
5f46165e6c51: Already exists
66220618f8db: Already exists
92f289eb2284: Pull complete
4f4fb700ef54: Pull complete
4c9f2742e959: Pull complete
9199260ef03e: Pull complete
806071d73b63: Pull complete
7b2ffaae0773: Pull complete
da3394aafcba: Pull complete
a02fd33b7bb9: Pull complete
f41b7d494800: Pull complete
339d0da2125f: Pull complete
741ce5d39413: Pull complete
137c00e264fd: Pull complete
de540e7b57fa: Pull complete
Digest: sha256:dbd2e0b3530f47457e64f5ed5f9cfeda7cd89aa09f9eeb0866cf156eb53de358
Status: Downloaded newer image for debezium/zookeeper:latest
Pulling kafka (debezium/kafka:latest)...
latest: Pulling from debezium/kafka
5f46165e6c51: Already exists
66220618f8db: Already exists
e027b0334c6a: Pull complete
66817e93921f: Pull complete
67d521eaed5d: Pull complete
cf708795d96d: Pull complete
fc3b8a67dc60: Pull complete
22dfac57eb73: Pull complete
463f309c9715: Pull complete
52fd63431d19: Pull complete
b7142045a660: Pull complete
260ed035bff1: Pull complete
4f4fb700ef54: Pull complete
7cb2d8b70bc3: Pull complete
Digest: sha256:3198c2f5a65648bf798a362e0c1b5fb7ac9e655ee07c02a5289687f45a8511be
Status: Downloaded newer image for debezium/kafka:latest
Creating project_zookeeper_1 ... done
Creating project_kafka_1     ... done
Creating project_connect_1   ... done
Attaching to project_zookeeper_1, project_kafka_1, project_connect_1
connect_1    | Using BOOTSTRAP_SERVERS=kafka:9092
connect_1    | Plugins are loaded from /usr/local/share/java,/usr/share/java
connect_1    | find: '/usr/local/share/java/': No such file or directory
kafka_1      | WARNING: Using default NODE_ID=1, which is valid only for non-clustered installations.
kafka_1      | Starting in ZooKeeper mode using NODE_ID=1.
zookeeper_1  | Starting up in standalone mode
zookeeper_1  | /usr/bin/java
zookeeper_1  | ZooKeeper JMX enabled by default
zookeeper_1  | Using config: /zookeeper/conf/zoo.cfg
zookeeper_1  | 2023-02-06 05:20:11,573 - INFO  [main:QuorumPeerConfig@174] - Reading configuration from: /zookeeper/conf/zoo.cfg
zookeeper_1  | 2023-02-06 05:20:11,576 - INFO  [main:QuorumPeerConfig@460] - clientPortAddress is 0.0.0.0:2181
zookeeper_1  | 2023-02-06 05:20:11,576 - INFO  [main:QuorumPeerConfig@464] - secureClientPort is not set
zookeeper_1  | 2023-02-06 05:20:11,576 - INFO  [main:QuorumPeerConfig@480] - observerMasterPort is not set
zookeeper_1  | 2023-02-06 05:20:11,576 - INFO  [main:QuorumPeerConfig@497] - metricsProvider.className is org.apache.zookeeper.metrics.impl.DefaultMetricsProvider
zookeeper_1  | 2023-02-06 05:20:11,578 - INFO  [main:DatadirCleanupManager@78] - autopurge.snapRetainCount set to 3
zookeeper_1  | 2023-02-06 05:20:11,578 - INFO  [main:DatadirCleanupManager@79] - autopurge.purgeInterval set to 1
zookeeper_1  | 2023-02-06 05:20:11,579 - WARN  [main:QuorumPeerMain@138] - Either no config or no quorum defined in config, running in standalone mode
kafka_1      | Using ZOOKEEPER_CONNECT=0.0.0.0:2181
kafka_1      | Using configuration config/server.properties.
kafka_1      | Using KAFKA_LISTENERS=PLAINTEXT://172.18.0.3:9092 and KAFKA_ADVERTISED_LISTENERS=PLAINTEXT://kafka:9092
zookeeper_1  | 2023-02-06 05:20:11,580 - INFO  [PurgeTask:DatadirCleanupManager$PurgeTask@139] - Purge task started.
zookeeper_1  | 2023-02-06 05:20:11,585 - INFO  [main:ManagedUtil@44] - Log4j 1.2 jmx support found and enabled.
zookeeper_1  | 2023-02-06 05:20:11,590 - INFO  [PurgeTask:FileTxnSnapLog@124] - zookeeper.snapshot.trust.empty : false
zookeeper_1  | 2023-02-06 05:20:11,598 - INFO  [main:QuorumPeerConfig@174] - Reading configuration from: /zookeeper/conf/zoo.cfg
zookeeper_1  | 2023-02-06 05:20:11,599 - INFO  [main:QuorumPeerConfig@460] - clientPortAddress is 0.0.0.0:2181
zookeeper_1  | 2023-02-06 05:20:11,599 - INFO  [main:QuorumPeerConfig@464] - secureClientPort is not set
zookeeper_1  | 2023-02-06 05:20:11,600 - INFO  [main:QuorumPeerConfig@480] - observerMasterPort is not set
zookeeper_1  | 2023-02-06 05:20:11,600 - INFO  [main:QuorumPeerConfig@497] - metricsProvider.className is org.apache.zookeeper.metrics.impl.DefaultMetricsProvider
zookeeper_1  | 2023-02-06 05:20:11,601 - INFO  [main:ZooKeeperServerMain@122] - Starting server
zookeeper_1  | 2023-02-06 05:20:11,600 - INFO  [PurgeTask:DatadirCleanupManager$PurgeTask@145] - Purge task completed.
zookeeper_1  | 2023-02-06 05:20:11,611 - INFO  [main:ServerMetrics@62] - ServerMetrics initialized with provider org.apache.zookeeper.metrics.impl.DefaultMetricsProvider@4ae3c1cd
zookeeper_1  | 2023-02-06 05:20:11,613 - INFO  [main:FileTxnSnapLog@124] - zookeeper.snapshot.trust.empty : false
zookeeper_1  | 2023-02-06 05:20:11,618 - INFO  [main:ZookeeperBanner@42] - 
zookeeper_1  | 2023-02-06 05:20:11,618 - INFO  [main:ZookeeperBanner@42] -   ______                  _                                          
zookeeper_1  | 2023-02-06 05:20:11,618 - INFO  [main:ZookeeperBanner@42] -  |___  /                 | |                                         
zookeeper_1  | 2023-02-06 05:20:11,618 - INFO  [main:ZookeeperBanner@42] -     / /    ___     ___   | | __   ___    ___   _ __     ___   _ __   
zookeeper_1  | 2023-02-06 05:20:11,618 - INFO  [main:ZookeeperBanner@42] -    / /    / _ \   / _ \  | |/ /  / _ \  / _ \ | '_ \   / _ \ | '__|
zookeeper_1  | 2023-02-06 05:20:11,618 - INFO  [main:ZookeeperBanner@42] -   / /__  | (_) | | (_) | |   <  |  __/ |  __/ | |_) | |  __/ | |    
zookeeper_1  | 2023-02-06 05:20:11,618 - INFO  [main:ZookeeperBanner@42] -  /_____|  \___/   \___/  |_|\_\  \___|  \___| | .__/   \___| |_|
zookeeper_1  | 2023-02-06 05:20:11,618 - INFO  [main:ZookeeperBanner@42] -                                               | |                     
zookeeper_1  | 2023-02-06 05:20:11,618 - INFO  [main:ZookeeperBanner@42] -                                               |_|                     
zookeeper_1  | 2023-02-06 05:20:11,618 - INFO  [main:ZookeeperBanner@42] - 
zookeeper_1  | 2023-02-06 05:20:11,619 - INFO  [main:Environment@98] - Server environment:zookeeper.version=3.6.3--6401e4ad2087061bc6b9f80dec2d69f2e3c8660a, built on 04/08/2021 16:35 GMT
zookeeper_1  | 2023-02-06 05:20:11,619 - INFO  [main:Environment@98] - Server environment:host.name=ab252c215487
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:java.version=11.0.18
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:java.vendor=Red Hat, Inc.
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:java.home=/usr/lib/jvm/java-11-openjdk-11.0.18.0.10-1.fc37.aarch64
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:java.class.path=/zookeeper/bin/../zookeeper-server/target/classes:/zookeeper/bin/../build/classes:/zookeeper/bin/../zookeeper-server/target/lib/*.jar:/zookeeper/bin/../build/lib/*.jar:/zookeeper/lib/zookeeper-prometheus-metrics-3.6.3.jar:/zookeeper/lib/zookeeper-jute-3.6.3.jar:/zookeeper/lib/zookeeper-3.6.3.jar:/zookeeper/lib/snappy-java-1.1.7.jar:/zookeeper/lib/slf4j-log4j12-1.7.25.jar:/zookeeper/lib/slf4j-api-1.7.25.jar:/zookeeper/lib/simpleclient_servlet-0.6.0.jar:/zookeeper/lib/simpleclient_hotspot-0.6.0.jar:/zookeeper/lib/simpleclient_common-0.6.0.jar:/zookeeper/lib/simpleclient-0.6.0.jar:/zookeeper/lib/netty-transport-native-unix-common-4.1.63.Final.jar:/zookeeper/lib/netty-transport-native-epoll-4.1.63.Final.jar:/zookeeper/lib/netty-transport-4.1.63.Final.jar:/zookeeper/lib/netty-resolver-4.1.63.Final.jar:/zookeeper/lib/netty-handler-4.1.63.Final.jar:/zookeeper/lib/netty-common-4.1.63.Final.jar:/zookeeper/lib/netty-codec-4.1.63.Final.jar:/zookeeper/lib/netty-buffer-4.1.63.Final.jar:/zookeeper/lib/metrics-core-3.2.5.jar:/zookeeper/lib/log4j-1.2.17.jar:/zookeeper/lib/json-simple-1.1.1.jar:/zookeeper/lib/jline-2.14.6.jar:/zookeeper/lib/jetty-util-ajax-9.4.39.v20210325.jar:/zookeeper/lib/jetty-util-9.4.39.v20210325.jar:/zookeeper/lib/jetty-servlet-9.4.39.v20210325.jar:/zookeeper/lib/jetty-server-9.4.39.v20210325.jar:/zookeeper/lib/jetty-security-9.4.39.v20210325.jar:/zookeeper/lib/jetty-io-9.4.39.v20210325.jar:/zookeeper/lib/jetty-http-9.4.39.v20210325.jar:/zookeeper/lib/javax.servlet-api-3.1.0.jar:/zookeeper/lib/jackson-databind-2.10.5.1.jar:/zookeeper/lib/jackson-core-2.10.5.jar:/zookeeper/lib/jackson-annotations-2.10.5.jar:/zookeeper/lib/commons-cli-1.2.jar:/zookeeper/lib/audience-annotations-0.5.0.jar:/zookeeper/bin/../zookeeper-*.jar:/zookeeper/bin/../zookeeper-server/src/main/resources/lib/*.jar:/zookeeper/conf:
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:java.library.path=/usr/java/packages/lib:/lib:/usr/lib:/usr/lib64:/lib64
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:java.io.tmpdir=/tmp
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:java.compiler=<NA>
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:os.name=Linux
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:os.arch=aarch64
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:os.version=5.10.104-linuxkit
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:user.name=zookeeper
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:user.home=/zookeeper
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:user.dir=/zookeeper
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:os.memory.free=111MB
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:os.memory.max=1000MB
zookeeper_1  | 2023-02-06 05:20:11,620 - INFO  [main:Environment@98] - Server environment:os.memory.total=126MB
zookeeper_1  | 2023-02-06 05:20:11,621 - INFO  [main:ZooKeeperServer@129] - zookeeper.enableEagerACLCheck = false
zookeeper_1  | 2023-02-06 05:20:11,621 - INFO  [main:ZooKeeperServer@137] - zookeeper.digest.enabled = true
zookeeper_1  | 2023-02-06 05:20:11,621 - INFO  [main:ZooKeeperServer@141] - zookeeper.closeSessionTxn.enabled = true
zookeeper_1  | 2023-02-06 05:20:11,621 - INFO  [main:ZooKeeperServer@1461] - zookeeper.flushDelay=0
zookeeper_1  | 2023-02-06 05:20:11,621 - INFO  [main:ZooKeeperServer@1470] - zookeeper.maxWriteQueuePollTime=0
zookeeper_1  | 2023-02-06 05:20:11,621 - INFO  [main:ZooKeeperServer@1479] - zookeeper.maxBatchSize=1000
zookeeper_1  | 2023-02-06 05:20:11,621 - INFO  [main:ZooKeeperServer@243] - zookeeper.intBufferStartingSizeBytes = 1024
zookeeper_1  | 2023-02-06 05:20:11,622 - INFO  [main:BlueThrottle@141] - Weighed connection throttling is disabled
zookeeper_1  | 2023-02-06 05:20:11,623 - INFO  [main:ZooKeeperServer@1273] - minSessionTimeout set to 4000
zookeeper_1  | 2023-02-06 05:20:11,623 - INFO  [main:ZooKeeperServer@1282] - maxSessionTimeout set to 40000
zookeeper_1  | 2023-02-06 05:20:11,623 - INFO  [main:ResponseCache@45] - Response cache size is initialized with value 400.
zookeeper_1  | 2023-02-06 05:20:11,623 - INFO  [main:ResponseCache@45] - Response cache size is initialized with value 400.
zookeeper_1  | 2023-02-06 05:20:11,624 - INFO  [main:RequestPathMetricsCollector@109] - zookeeper.pathStats.slotCapacity = 60
zookeeper_1  | 2023-02-06 05:20:11,624 - INFO  [main:RequestPathMetricsCollector@110] - zookeeper.pathStats.slotDuration = 15
zookeeper_1  | 2023-02-06 05:20:11,624 - INFO  [main:RequestPathMetricsCollector@111] - zookeeper.pathStats.maxDepth = 6
zookeeper_1  | 2023-02-06 05:20:11,624 - INFO  [main:RequestPathMetricsCollector@112] - zookeeper.pathStats.initialDelay = 5
zookeeper_1  | 2023-02-06 05:20:11,624 - INFO  [main:RequestPathMetricsCollector@113] - zookeeper.pathStats.delay = 5
zookeeper_1  | 2023-02-06 05:20:11,624 - INFO  [main:RequestPathMetricsCollector@114] - zookeeper.pathStats.enabled = false
zookeeper_1  | 2023-02-06 05:20:11,626 - INFO  [main:ZooKeeperServer@1498] - The max bytes for all large requests are set to 104857600
zookeeper_1  | 2023-02-06 05:20:11,626 - INFO  [main:ZooKeeperServer@1512] - The large request threshold is set to -1
zookeeper_1  | 2023-02-06 05:20:11,626 - INFO  [main:ZooKeeperServer@339] - Created server with tickTime 2000 minSessionTimeout 4000 maxSessionTimeout 40000 clientPortListenBacklog -1 datadir /zookeeper/txns/version-2 snapdir /zookeeper/data/version-2
zookeeper_1  | 2023-02-06 05:20:11,655 - INFO  [main:Log@169] - Logging initialized @362ms to org.eclipse.jetty.util.log.Slf4jLog
zookeeper_1  | 2023-02-06 05:20:11,706 - WARN  [main:ContextHandler@1660] - o.e.j.s.ServletContextHandler@77888435{/,null,STOPPED} contextPath ends with /*
zookeeper_1  | 2023-02-06 05:20:11,707 - WARN  [main:ContextHandler@1671] - Empty contextPath
zookeeper_1  | 2023-02-06 05:20:11,731 - INFO  [main:Server@375] - jetty-9.4.39.v20210325; built: 2021-03-25T14:42:11.471Z; git: 9fc7ca5a922f2a37b84ec9dbc26a5168cee7e667; jvm 11.0.18+10
zookeeper_1  | 2023-02-06 05:20:11,780 - INFO  [main:DefaultSessionIdManager@334] - DefaultSessionIdManager workerName=node0
zookeeper_1  | 2023-02-06 05:20:11,781 - INFO  [main:DefaultSessionIdManager@339] - No SessionScavenger set, using defaults
zookeeper_1  | 2023-02-06 05:20:11,783 - INFO  [main:HouseKeeper@132] - node0 Scavenging every 660000ms
zookeeper_1  | 2023-02-06 05:20:11,786 - WARN  [main:ConstraintSecurityHandler@759] - ServletContext@o.e.j.s.ServletContextHandler@77888435{/,null,STARTING} has uncovered http methods for path: /*
zookeeper_1  | 2023-02-06 05:20:11,807 - INFO  [main:ContextHandler@916] - Started o.e.j.s.ServletContextHandler@77888435{/,null,AVAILABLE}
zookeeper_1  | 2023-02-06 05:20:11,833 - INFO  [main:AbstractConnector@331] - Started ServerConnector@42e99e4a{HTTP/1.1, (http/1.1)}{0.0.0.0:8080}
zookeeper_1  | 2023-02-06 05:20:11,833 - INFO  [main:Server@415] - Started @540ms
zookeeper_1  | 2023-02-06 05:20:11,834 - INFO  [main:JettyAdminServer@191] - Started AdminServer on address 0.0.0.0, port 8080 and command URL /commands
zookeeper_1  | 2023-02-06 05:20:11,838 - INFO  [main:ServerCnxnFactory@169] - Using org.apache.zookeeper.server.NIOServerCnxnFactory as server connection factory
zookeeper_1  | 2023-02-06 05:20:11,839 - WARN  [main:ServerCnxnFactory@309] - maxCnxns is not configured, using default value 0.
zookeeper_1  | 2023-02-06 05:20:11,841 - INFO  [main:NIOServerCnxnFactory@666] - Configuring NIO connection handler with 10s sessionless connection timeout, 1 selector thread(s), 10 worker threads, and 64 kB direct buffers.
zookeeper_1  | 2023-02-06 05:20:11,842 - INFO  [main:NIOServerCnxnFactory@674] - binding to port 0.0.0.0/0.0.0.0:2181
zookeeper_1  | 2023-02-06 05:20:11,856 - INFO  [main:WatchManagerFactory@42] - Using org.apache.zookeeper.server.watch.WatchManager as watch manager
zookeeper_1  | 2023-02-06 05:20:11,856 - INFO  [main:WatchManagerFactory@42] - Using org.apache.zookeeper.server.watch.WatchManager as watch manager
zookeeper_1  | 2023-02-06 05:20:11,857 - INFO  [main:ZKDatabase@132] - zookeeper.snapshotSizeFactor = 0.33
zookeeper_1  | 2023-02-06 05:20:11,857 - INFO  [main:ZKDatabase@152] - zookeeper.commitLogCount=500
zookeeper_1  | 2023-02-06 05:20:11,862 - INFO  [main:SnapStream@61] - zookeeper.snapshot.compression.method = CHECKED
zookeeper_1  | 2023-02-06 05:20:11,862 - INFO  [main:FileTxnSnapLog@470] - Snapshotting: 0x0 to /zookeeper/data/version-2/snapshot.0
zookeeper_1  | 2023-02-06 05:20:11,864 - INFO  [main:ZKDatabase@289] - Snapshot loaded in 8 ms, highest zxid is 0x0, digest is 1371985504
zookeeper_1  | 2023-02-06 05:20:11,865 - INFO  [main:FileTxnSnapLog@470] - Snapshotting: 0x0 to /zookeeper/data/version-2/snapshot.0
zookeeper_1  | 2023-02-06 05:20:11,866 - INFO  [main:ZooKeeperServer@529] - Snapshot taken in 1 ms
zookeeper_1  | 2023-02-06 05:20:11,873 - INFO  [main:RequestThrottler@74] - zookeeper.request_throttler.shutdownTimeout = 10000
zookeeper_1  | 2023-02-06 05:20:11,873 - INFO  [ProcessThread(sid:0 cport:2181)::PrepRequestProcessor@136] - PrepRequestProcessor (sid:0) started, reconfigEnabled=false
zookeeper_1  | 2023-02-06 05:20:11,901 - INFO  [main:ContainerManager@83] - Using checkIntervalMs=60000 maxPerMinute=10000 maxNeverUsedIntervalMs=0
zookeeper_1  | 2023-02-06 05:20:11,903 - INFO  [main:ZKAuditProvider@42] - ZooKeeper audit is disabled.
project_connect_1 exited with code 1
kafka_1      | 2023-02-06 05:20:12,406 - INFO  [main:Log4jControllerRegistration$@31] - Registered kafka:type=kafka.Log4jController MBean
kafka_1      | 2023-02-06 05:20:12,554 - INFO  [main:X509Util@77] - Setting -D jdk.tls.rejectClientInitiatedRenegotiation=true to disable client-initiated TLS renegotiation
kafka_1      | 2023-02-06 05:20:12,596 - INFO  [main:LoggingSignalHandler@72] - Registered signal handlers for TERM, INT, HUP
kafka_1      | 2023-02-06 05:20:12,597 - INFO  [main:Logging@66] - starting
kafka_1      | 2023-02-06 05:20:12,597 - INFO  [main:Logging@66] - Connecting to zookeeper on 0.0.0.0:2181
kafka_1      | 2023-02-06 05:20:12,613 - INFO  [main:Logging@66] - [ZooKeeperClient Kafka server] Initializing a new session to 0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:zookeeper.version=3.6.3--6401e4ad2087061bc6b9f80dec2d69f2e3c8660a, built on 04/08/2021 16:35 GMT
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:host.name=b636f3112eff
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:java.version=11.0.18
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:java.vendor=Red Hat, Inc.
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:java.home=/usr/lib/jvm/java-11-openjdk-11.0.18.0.10-1.fc37.aarch64
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:java.class.path=/kafka/libs/activation-1.1.1.jar:/kafka/libs/aopalliance-repackaged-2.6.1.jar:/kafka/libs/argparse4j-0.7.0.jar:/kafka/libs/audience-annotations-0.5.0.jar:/kafka/libs/commons-cli-1.4.jar:/kafka/libs/commons-lang3-3.12.0.jar:/kafka/libs/commons-lang3-3.8.1.jar:/kafka/libs/connect-api-3.3.1.jar:/kafka/libs/connect-basic-auth-extension-3.3.1.jar:/kafka/libs/connect-json-3.3.1.jar:/kafka/libs/connect-mirror-3.3.1.jar:/kafka/libs/connect-mirror-client-3.3.1.jar:/kafka/libs/connect-runtime-3.3.1.jar:/kafka/libs/connect-transforms-3.3.1.jar:/kafka/libs/hk2-api-2.6.1.jar:/kafka/libs/hk2-locator-2.6.1.jar:/kafka/libs/hk2-utils-2.6.1.jar:/kafka/libs/jackson-annotations-2.13.3.jar:/kafka/libs/jackson-core-2.13.3.jar:/kafka/libs/jackson-databind-2.13.3.jar:/kafka/libs/jackson-dataformat-csv-2.13.3.jar:/kafka/libs/jackson-datatype-jdk8-2.13.3.jar:/kafka/libs/jackson-jaxrs-base-2.13.3.jar:/kafka/libs/jackson-jaxrs-json-provider-2.13.3.jar:/kafka/libs/jackson-module-jaxb-annotations-2.13.3.jar:/kafka/libs/jackson-module-scala_2.13-2.13.3.jar:/kafka/libs/jakarta.activation-api-1.2.2.jar:/kafka/libs/jakarta.annotation-api-1.3.5.jar:/kafka/libs/jakarta.inject-2.6.1.jar:/kafka/libs/jakarta.validation-api-2.0.2.jar:/kafka/libs/jakarta.ws.rs-api-2.1.6.jar:/kafka/libs/jakarta.xml.bind-api-2.3.3.jar:/kafka/libs/javassist-3.27.0-GA.jar:/kafka/libs/javax.servlet-api-3.1.0.jar:/kafka/libs/javax.ws.rs-api-2.1.1.jar:/kafka/libs/jaxb-api-2.3.0.jar:/kafka/libs/jersey-client-2.34.jar:/kafka/libs/jersey-common-2.34.jar:/kafka/libs/jersey-container-servlet-2.34.jar:/kafka/libs/jersey-container-servlet-core-2.34.jar:/kafka/libs/jersey-hk2-2.34.jar:/kafka/libs/jersey-server-2.34.jar:/kafka/libs/jetty-client-9.4.48.v20220622.jar:/kafka/libs/jetty-continuation-9.4.48.v20220622.jar:/kafka/libs/jetty-http-9.4.48.v20220622.jar:/kafka/libs/jetty-io-9.4.48.v20220622.jar:/kafka/libs/jetty-security-9.4.48.v20220622.jar:/kafka/libs/jetty-server-9.4.48.v20220622.jar:/kafka/libs/jetty-servlet-9.4.48.v20220622.jar:/kafka/libs/jetty-servlets-9.4.48.v20220622.jar:/kafka/libs/jetty-util-9.4.48.v20220622.jar:/kafka/libs/jetty-util-ajax-9.4.48.v20220622.jar:/kafka/libs/jline-3.21.0.jar:/kafka/libs/jopt-simple-5.0.4.jar:/kafka/libs/jose4j-0.7.9.jar:/kafka/libs/kafka-clients-3.3.1.jar:/kafka/libs/kafka-log4j-appender-3.3.1.jar:/kafka/libs/kafka-metadata-3.3.1.jar:/kafka/libs/kafka-raft-3.3.1.jar:/kafka/libs/kafka-server-common-3.3.1.jar:/kafka/libs/kafka-shell-3.3.1.jar:/kafka/libs/kafka-storage-3.3.1.jar:/kafka/libs/kafka-storage-api-3.3.1.jar:/kafka/libs/kafka-streams-3.3.1.jar:/kafka/libs/kafka-streams-examples-3.3.1.jar:/kafka/libs/kafka-streams-scala_2.13-3.3.1.jar:/kafka/libs/kafka-streams-test-utils-3.3.1.jar:/kafka/libs/kafka-tools-3.3.1.jar:/kafka/libs/kafka_2.13-3.3.1.jar:/kafka/libs/lz4-java-1.8.0.jar:/kafka/libs/maven-artifact-3.8.4.jar:/kafka/libs/metrics-core-2.2.0.jar:/kafka/libs/metrics-core-4.1.12.1.jar:/kafka/libs/netty-buffer-4.1.78.Final.jar:/kafka/libs/netty-codec-4.1.78.Final.jar:/kafka/libs/netty-common-4.1.78.Final.jar:/kafka/libs/netty-handler-4.1.78.Final.jar:/kafka/libs/netty-resolver-4.1.78.Final.jar:/kafka/libs/netty-transport-4.1.78.Final.jar:/kafka/libs/netty-transport-classes-epoll-4.1.78.Final.jar:/kafka/libs/netty-transport-native-epoll-4.1.78.Final.jar:/kafka/libs/netty-transport-native-unix-common-4.1.78.Final.jar:/kafka/libs/osgi-resource-locator-1.0.3.jar:/kafka/libs/paranamer-2.8.jar:/kafka/libs/plexus-utils-3.3.0.jar:/kafka/libs/reflections-0.9.12.jar:/kafka/libs/reload4j-1.2.19.jar:/kafka/libs/rocksdbjni-6.29.4.1.jar:/kafka/libs/scala-collection-compat_2.13-2.6.0.jar:/kafka/libs/scala-java8-compat_2.13-1.0.2.jar:/kafka/libs/scala-library-2.13.8.jar:/kafka/libs/scala-logging_2.13-3.9.4.jar:/kafka/libs/scala-reflect-2.13.8.jar:/kafka/libs/slf4j-api-1.7.36.jar:/kafka/libs/slf4j-reload4j-1.7.36.jar:/kafka/libs/snappy-java-1.1.8.4.jar:/kafka/libs/swagger-annotations-2.2.0.jar:/kafka/libs/trogdor-3.3.1.jar:/kafka/libs/zookeeper-3.6.3.jar:/kafka/libs/zookeeper-jute-3.6.3.jar:/kafka/libs/zstd-jni-1.5.2-1.jar
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:java.library.path=/usr/java/packages/lib:/lib:/usr/lib:/usr/lib64:/lib64
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:java.io.tmpdir=/tmp
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:java.compiler=<NA>
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:os.name=Linux
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:os.arch=aarch64
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:os.version=5.10.104-linuxkit
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:user.name=kafka
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:user.home=/kafka
kafka_1      | 2023-02-06 05:20:12,616 - INFO  [main:Environment@98] - Client environment:user.dir=/kafka
kafka_1      | 2023-02-06 05:20:12,617 - INFO  [main:Environment@98] - Client environment:os.memory.free=1015MB
kafka_1      | 2023-02-06 05:20:12,617 - INFO  [main:Environment@98] - Client environment:os.memory.max=1024MB
kafka_1      | 2023-02-06 05:20:12,617 - INFO  [main:Environment@98] - Client environment:os.memory.total=1024MB
kafka_1      | 2023-02-06 05:20:12,618 - INFO  [main:ZooKeeper@1006] - Initiating client connection, connectString=0.0.0.0:2181 sessionTimeout=18000 watcher=kafka.zookeeper.ZooKeeperClient$ZooKeeperClientWatcher$@64e7619d
kafka_1      | 2023-02-06 05:20:12,621 - INFO  [main:ClientCnxnSocket@239] - jute.maxbuffer value is 4194304 Bytes
kafka_1      | 2023-02-06 05:20:12,623 - INFO  [main:ClientCnxn@1736] - zookeeper.request.timeout value is 0. feature enabled=false
kafka_1      | 2023-02-06 05:20:12,628 - INFO  [main:Logging@66] - [ZooKeeperClient Kafka server] Waiting until connected.
kafka_1      | 2023-02-06 05:20:12,628 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:12,636 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:13,750 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:13,752 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:14,858 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:14,861 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:15,973 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:15,975 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:17,085 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:17,090 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:18,209 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:18,213 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:19,322 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:19,326 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:20,439 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:20,442 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:21,546 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:21,548 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:22,652 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:22,653 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:23,758 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:23,760 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:24,870 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:24,871 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:25,975 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:25,984 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:27,092 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:27,094 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:28,204 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:28,207 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:29,317 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:29,321 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:30,448 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:30,452 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1300] - Session 0x0 for sever /0.0.0.0:2181, Closing socket connection. Attempting reconnect except it is a SessionExpiredException.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:30,633 - INFO  [main:Logging@66] - [ZooKeeperClient Kafka server] Closing.
kafka_1      | 2023-02-06 05:20:31,566 - INFO  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1181] - Opening socket connection to server /0.0.0.0:2181.
kafka_1      | 2023-02-06 05:20:31,580 - WARN  [main-SendThread(0.0.0.0:2181):ClientCnxn$SendThread@1294] - An exception was thrown while closing send thread for session 0x0.
kafka_1      | java.net.ConnectException: Connection refused
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.checkConnect(Native Method)
kafka_1      |  at java.base/sun.nio.ch.SocketChannelImpl.finishConnect(SocketChannelImpl.java:777)
kafka_1      |  at org.apache.zookeeper.ClientCnxnSocketNIO.doTransport(ClientCnxnSocketNIO.java:344)
kafka_1      |  at org.apache.zookeeper.ClientCnxn$SendThread.run(ClientCnxn.java:1290)
kafka_1      | 2023-02-06 05:20:31,700 - INFO  [main:ZooKeeper@1619] - Session: 0x0 closed
kafka_1      | 2023-02-06 05:20:31,704 - INFO  [main-EventThread:ClientCnxn$EventThread@578] - EventThread shut down for session: 0x0
kafka_1      | 2023-02-06 05:20:31,708 - INFO  [main:Logging@66] - [ZooKeeperClient Kafka server] Closed.
kafka_1      | 2023-02-06 05:20:31,713 - ERROR [main:MarkerIgnoringBase@159] - Fatal error during KafkaServer startup. Prepare to shutdown
kafka_1      | kafka.zookeeper.ZooKeeperClientTimeoutException: Timed out waiting for connection while in state: CONNECTING
kafka_1      |  at kafka.zookeeper.ZooKeeperClient.waitUntilConnected(ZooKeeperClient.scala:254)
kafka_1      |  at kafka.zookeeper.ZooKeeperClient.<init>(ZooKeeperClient.scala:108)
kafka_1      |  at kafka.zk.KafkaZkClient$.apply(KafkaZkClient.scala:1980)
kafka_1      |  at kafka.server.KafkaServer.initZkClient(KafkaServer.scala:503)
kafka_1      |  at kafka.server.KafkaServer.startup(KafkaServer.scala:203)
kafka_1      |  at kafka.Kafka$.main(Kafka.scala:109)
kafka_1      |  at kafka.Kafka.main(Kafka.scala)
kafka_1      | 2023-02-06 05:20:31,714 - INFO  [main:Logging@66] - shutting down
kafka_1      | 2023-02-06 05:20:31,724 - INFO  [main:AppInfoParser@83] - App info kafka.server for 1 unregistered
kafka_1      | 2023-02-06 05:20:31,725 - INFO  [main:Logging@66] - shut down completed
kafka_1      | 2023-02-06 05:20:31,725 - ERROR [main:MarkerIgnoringBase@159] - Exiting Kafka due to fatal exception during startup.
kafka_1      | kafka.zookeeper.ZooKeeperClientTimeoutException: Timed out waiting for connection while in state: CONNECTING
kafka_1      |  at kafka.zookeeper.ZooKeeperClient.waitUntilConnected(ZooKeeperClient.scala:254)
kafka_1      |  at kafka.zookeeper.ZooKeeperClient.<init>(ZooKeeperClient.scala:108)
kafka_1      |  at kafka.zk.KafkaZkClient$.apply(KafkaZkClient.scala:1980)
kafka_1      |  at kafka.server.KafkaServer.initZkClient(KafkaServer.scala:503)
kafka_1      |  at kafka.server.KafkaServer.startup(KafkaServer.scala:203)
kafka_1      |  at kafka.Kafka$.main(Kafka.scala:109)
kafka_1      |  at kafka.Kafka.main(Kafka.scala)
kafka_1      | 2023-02-06 05:20:31,728 - INFO  [kafka-shutdown-hook:Logging@66] - shutting down
project_kafka_1 exited with code 1
