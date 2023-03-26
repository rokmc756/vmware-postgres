## What is PostgreSQL Cluster
postgres-cluster provide ansible playbook to deploy three kind of clusters such as gpfailover, patroni cluster, mutlti master replication ( bdr ).

## patroni cluster
https://github.com/rokmc756/postgres-cluster/tree/main/roles/vmware-patroni

## pg_auto_failover cluster
https://github.com/rokmc756/postgres-cluster/tree/main/roles/vmware-pgautofailover

## Reference links
https://www.techsupportpk.com/2020/02/how-to-create-highly-available-postgresql-cluster-using-patroni-haproxy-centos-rhel-7.html



## Error with sync mode
~~~
  File "/usr/lib/python3.6/site-packages/patroni/ha.py", line 1277, in _run_cycle
    return self.post_bootstrap()
  File "/usr/lib/python3.6/site-packages/patroni/ha.py", line 1173, in post_bootstrap
    self.cancel_initialization()
  File "/usr/lib/python3.6/site-packages/patroni/ha.py", line 1168, in cancel_initialization
    raise PatroniException('Failed to bootstrap cluster')
patroni.exceptions.PatroniException: 'Failed to bootstrap cluster'
~~~

## Replication modes
~~~
https://patroni.readthedocs.io/en/latest/replication_modes.html
~~~

## Replica imaging and bootstrap
~~~
https://patroni.readthedocs.io/en/latest/replica_bootstrap.html
~~~
