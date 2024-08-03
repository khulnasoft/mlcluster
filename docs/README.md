<!-- markdownlint-disable -->

# API Overview

## Modules

- [`mlcluster.cluster`](./mlcluster.cluster.md#module-mlclustercluster)
- [`mlcluster.cluster.dask_cluster`](./mlcluster.cluster.dask_cluster.md#module-mlclusterclusterdask_cluster): Module for conveniently managing a [DASK](http://distributed.dask.org) cluster.
- [`mlcluster.cluster.exceptions`](./mlcluster.cluster.exceptions.md#module-mlclusterclusterexceptions): Exception module for cluster classes.
- [`mlcluster.cluster.hyperopt_cluster`](./mlcluster.cluster.hyperopt_cluster.md#module-mlclusterclusterhyperopt_cluster): Module for conveniently managing a [Hyperopt](https://github.com/hyperopt/hyperopt) cluster.
- [`mlcluster.cluster.runtime_cluster`](./mlcluster.cluster.runtime_cluster.md#module-mlclusterclusterruntime_cluster): Module comprising the abstract RuntimeCluster class with its related `launcher strategy` classes.
- [`mlcluster.exceptions`](./mlcluster.exceptions.md#module-mlclusterexceptions): Exception module.
- [`mlcluster.runtime_mgmt`](./mlcluster.runtime_mgmt.md#module-mlclusterruntime_mgmt): Runtime management module. This module contains convenient classes for working with `Runtimes` and `RuntimeTasks`.
- [`mlcluster.runtimes`](./mlcluster.runtimes.md#module-mlclusterruntimes): Runtimes module.
- [`mlcluster.scripts`](./mlcluster.scripts.md#module-mlclusterscripts)
- [`mlcluster.scripts.cli_handler`](./mlcluster.scripts.cli_handler.md#module-mlclusterscriptscli_handler)
- [`mlcluster.settings`](./mlcluster.settings.md#module-mlclustersettings): Contains setting parameters for the library.
- [`mlcluster.utils`](./mlcluster.utils.md#module-mlclusterutils)

## Classes

- [`dask_cluster.DaskCluster`](./mlcluster.cluster.dask_cluster.md#class-daskcluster): Convenient class for launching a Dask cluster in a `RuntimeGroup`.
- [`dask_cluster.LocalMasterLauncher`](./mlcluster.cluster.dask_cluster.md#class-localmasterlauncher): Concrete implementation of the `MasterLauncher` interface. See its documentation to get a list of the inherited methods and attributes.
- [`dask_cluster.RoundRobinLauncher`](./mlcluster.cluster.dask_cluster.md#class-roundrobinlauncher): WorkerLauncher implementation for launching DASK workers in a round robin manner. See its documentation to get a list of the inherited methods and attributes.
- [`exceptions.MasterStartError`](./mlcluster.cluster.exceptions.md#class-masterstarterror): Error indicating that the cluster master instance could not be started successfully.
- [`hyperopt_cluster.HyperoptCluster`](./mlcluster.cluster.hyperopt_cluster.md#class-hyperoptcluster): Convenient class for launching a Hyperopt cluster in a `RuntimeGroup`.
- [`hyperopt_cluster.LocalMongoLauncher`](./mlcluster.cluster.hyperopt_cluster.md#class-localmongolauncher): Concrete implementation of the `MasterLauncher` interface. See its documentation to get a list of the inherited methods and attributes.
- [`hyperopt_cluster.MongoLauncher`](./mlcluster.cluster.hyperopt_cluster.md#class-mongolauncher): Abstract implementation of the `MasterLauncher` interface used to implement a concrete launch strategy for mongodb instance used in hyperopt.
- [`hyperopt_cluster.RoundRobinLauncher`](./mlcluster.cluster.hyperopt_cluster.md#class-roundrobinlauncher): Concrete WorkerLauncher implementation for launching hyperopt workers in a round robin manner.
- [`runtime_cluster.MasterLauncher`](./mlcluster.cluster.runtime_cluster.md#class-masterlauncher): Abstract class for implementing the strategy for launching the master instance of the cluster.
- [`runtime_cluster.MasterWorkerCluster`](./mlcluster.cluster.runtime_cluster.md#class-masterworkercluster): Class for clusters following a master-worker architecture.
- [`runtime_cluster.RuntimeCluster`](./mlcluster.cluster.runtime_cluster.md#class-runtimecluster): Abstract cluster class.
- [`runtime_cluster.WorkerLauncher`](./mlcluster.cluster.runtime_cluster.md#class-workerlauncher): Abstract class for implementing the strategy for launching worker instances within a RuntimeGroup.
- [`exceptions.InvalidRuntimeError`](./mlcluster.exceptions.md#class-invalidruntimeerror): Error indicating that a `Runtime` can not be instantiated properly.
- [`exceptions.MlclusterError`](./mlcluster.exceptions.md#class-mlclustererror): Basic exception class for `mlcluster` library errors.
- [`exceptions.NoPortsLeftError`](./mlcluster.exceptions.md#class-noportslefterror): Error indicating that there are no more ports left from the given port list.
- [`exceptions.NoRuntimesDetectedError`](./mlcluster.exceptions.md#class-noruntimesdetectederror): Error indicating that no `Runtime` could be detcted automatically by a `RuntimeManager` for example.
- [`exceptions.PathCreationError`](./mlcluster.exceptions.md#class-pathcreationerror): Error indicating that a given path could not be created.
- [`exceptions.PortInUseError`](./mlcluster.exceptions.md#class-portinuseerror): Error indicating that a port is already in use in a `RuntimeGroup` or on the local machine.
- [`exceptions.TaskExecutionError`](./mlcluster.exceptions.md#class-taskexecutionerror): This error relates to exceptions occured during RuntimeTask execution.
- [`runtime_mgmt.RuntimeGroup`](./mlcluster.runtime_mgmt.md#class-runtimegroup): A `RuntimeGroup` is the representation of logically related `Runtimes`.
- [`runtime_mgmt.RuntimeManager`](./mlcluster.runtime_mgmt.md#class-runtimemanager): The `RuntimeManager` can be used for a simplified resource management.
- [`runtimes.Runtime`](./mlcluster.runtimes.md#class-runtime): A `Runtime` is the logical representation of a remote host.
- [`runtimes.RuntimeTask`](./mlcluster.runtimes.md#class-runtimetask): This class provides the functionality for executing a sequence of elementary operations over ssh.
- [`utils.Environment`](./mlcluster.utils.md#class-environment): This class contains environment variables.
- [`utils.ExecutionFileLogUtil`](./mlcluster.utils.md#class-executionfilelogutil): Generic class used to write log files.
- [`utils.Timestamp`](./mlcluster.utils.md#class-timestamp): Custom Timestamp class with convenient methods.

## Functions

- No functions


---

_This file was automatically generated via [lazydocs](https://github.com/khulnasoft/lazydocs)._
