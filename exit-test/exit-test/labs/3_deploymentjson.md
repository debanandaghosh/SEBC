


[root@instance-2 yum.repos.d]# curl -u admin:admin "http://localhost:7180/api/v5/hosts"
{
  "items" : [ {
    "hostId" : "ced12e1d-c508-4401-81cb-4f21fc6dbe59",
    "ipAddress" : "10.142.0.2",
    "hostname" : "instance-1.c.golden-veld-204308.internal",
    "rackId" : "/default",
    "hostUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/hostRedirect/ced12e1d-c508-4401-81cb-4f21fc6dbe59",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 15600513024
  }, {
    "hostId" : "b92c8197-ebf4-43ee-a8be-d88be3f5ce68",
    "ipAddress" : "10.142.0.3",
    "hostname" : "instance-2.c.golden-veld-204308.internal",
    "rackId" : "/default",
    "hostUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/hostRedirect/b92c8197-ebf4-43ee-a8be-d88be3f5ce68",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 15600513024
  }, {
    "hostId" : "206c0fa3-9414-4ec7-a720-9a317da2f79a",
    "ipAddress" : "10.128.0.2",
    "hostname" : "instance-3.c.golden-veld-204308.internal",
    "rackId" : "/default",
    "hostUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/hostRedirect/206c0fa3-9414-4ec7-a720-9a317da2f79a",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 15600504832
  }, {
    "hostId" : "da2984d6-572b-4854-8478-1aba0f37c31a",
    "ipAddress" : "10.128.0.3",
    "hostname" : "instance-4.c.golden-veld-204308.internal",
    "rackId" : "/default",
    "hostUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/hostRedirect/da2984d6-572b-4854-8478-1aba0f37c31a",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 15600504832
  }, {
    "hostId" : "61a842f7-b567-4e21-9634-d3e089ee5c89",
    "ipAddress" : "10.138.0.2",
    "hostname" : "instance-5.c.golden-veld-204308.internal",
    "rackId" : "/default",
    "hostUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/hostRedirect/61a842f7-b567-4e21-9634-d3e089ee5c89",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "totalPhysMemBytes" : 15600513024
  } ]
}[root@instance-2 yum.repos.d]# 

[root@instance-2 yum.repos.d]# curl -u admin:admin "http://localhost:7180/api/v11/clusters/debanandaghosh/services"
{
  "items" : [ {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/zookeeper",
    "roleInstancesUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/zookeeper/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "STALE",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/hdfs",
    "roleInstancesUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/hdfs/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : true
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "STALE",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HDFS",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "mapreduce",
    "type" : "MAPREDUCE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/mapreduce",
    "roleInstancesUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/mapreduce/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "MAPREDUCE_HA_JOB_TRACKER_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "MAPREDUCE_TASK_TRACKERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "MapReduce",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/oozie",
    "roleInstancesUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/oozie/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hive",
    "type" : "HIVE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/hive",
    "roleInstancesUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/hive/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HIVE_HIVEMETASTORES_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HIVE_HIVESERVER2S_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "impala",
    "type" : "IMPALA",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/impala",
    "roleInstancesUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/impala/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "IMPALA_ASSIGNMENT_LOCALITY",
      "summary" : "DISABLED",
      "suppressed" : false
    }, {
      "name" : "IMPALA_CATALOGSERVER_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "IMPALA_IMPALADS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "IMPALA_STATESTORE_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Impala",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/hue",
    "roleInstancesUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/hue/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hbase",
    "type" : "HBASE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/hbase",
    "roleInstancesUrl" : "http://instance-2.c.golden-veld-204308.internal:7180/cmf/serviceRedirect/hbase/instances",
    "serviceState" : "STOPPED",
    "healthSummary" : "DISABLED",
    "healthChecks" : [ {
      "name" : "HBASE_MASTER_HEALTH",
      "summary" : "DISABLED",
      "suppressed" : false
    }, {
      "name" : "HBASE_REGION_SERVERS_HEALTHY",
      "summary" : "DISABLED",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "STALE",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HBase",
    "entityStatus" : "STOPPED"
  } ]


