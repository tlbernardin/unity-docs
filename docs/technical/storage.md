# Storage

Below if a table of all available storage on Unity.

| Mountpoint | Name                | Location                          | Type     | Quota                                   | Description                                                                                                                                                                                                                                                                                                                                                                              |
| ---------- | ------------------- | --------------------------------- | -------- | --------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| /home      | Home directories    | Everywhere                        | HDD      | 50 GB                                   | Home directories should be used only for user init files.                                                                                                                                                                                                 
| /work/pi_      | Work directories    | Everywhere                        | SSD      | 1 TB                                  | Work should be used as the primary location for running cluster jobs. This is a shared folder for all users in the PI group. /work/username, is a legacy directory available to older users which is being phased out.
| /project  | Project directories | Everywhere                        | HDD      | As Needed                                 | Project directories are available to PI's upon request. Good for large dataset storage or any larger storage that is not directly used for job I/O. PI's should e-mail hpc@umass.edu to request. A common use case is generating job output in /work and copying to permanent storage in /project afterwards. **Not for job I/O**                                                                                 |
| /nese      | NESE mounts         | Everywhere                        | HDD/Tape | Varying                                 | Legacy images available from the northeast storage exchange can be found here. **Not for job I/O**                                                                                                          |
| /nas       | Buy-in NAS mounts   | Everywhere                        | Varying  | Varying                                 | Legacy location where the mounts for buy-in NAS hardware are located on Unity. For users who purchased storage nodes for their own use on Unity only.                                                                                                                                                                                                                                    |
| /scratch   | Scratch space       | Everywhere (Intended for Compute) | SSD      | 40 TB / user, cleared at the end of job | /scratch/[nodeid]/[jobid] is created when a job is started. That folder is assigned to $TMP and deleted after the job is complete. This directory is not directly available to users. |
| /gypsum    | Gypsum devices      | Everywhere                        | HDD      | Varying                                 | For users migrating from the Gypsum cluster to the Unity clusters, you will find all your old storage here.                                                                                                                                                                                                                                                                              |
| /old       | Old mounts          | Everywhere (Read-Only)            | Varying  | Varying                                 | Old filesystems which are deprecated live here until they are deleted.                                                                                                                                                                                                                                                                                                                   |