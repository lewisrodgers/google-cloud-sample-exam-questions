# cloud-architect-18

To reduce costs, the Director of Engineering has required all developers to move their development infrastructure resources from on-premises virtual machines (VMs) to Google Cloud. These resources go through multiple start/stop events during the day and require state to persist. You have been asked to design the process of running a development environment in Google Cloud while providing cost visibility to the finance department. Which two steps should you take? (Choose two)

A. Use persistent disks to store the state. Start and stop the VM as needed.

B. Use the "gcloud --auto-delete" flag on all persistent disks before stopping the VM.

C. Apply VM CPU utilization label and include it in the BigQuery billing export.

D. Use BigQuery billing export and labels to relate cost to groups.

E. Store all state in a Local SSD, snapshot the persistent disks, and terminate the VM.

## Feedback

A is correct because persistent disks will not be deleted when an instance is stopped.

B is not correct because the --auto-delete flag has no effect unless the instance is deleted. Stopping an instance does not delete the instance or the attached persistent disks.

C is not correct because labels are used to organize instances, not to monitor metrics.

D is correct because exporting daily usage and cost estimates automatically throughout the day to a BigQuery dataset is a good way of providing visibility to the finance department. Labels can then be used to group the costs based on team or cost center.

E is not correct because the state stored in local SSDs will be lost when the instance is stopped.

https://cloud.google.com/compute/docs/instances/instance-life-cycle

https://cloud.google.com/sdk/gcloud/reference/compute/instances/set-disk-auto-delete#--auto-delete

https://cloud.google.com/sdk/gcloud/reference/compute/instances/create#--disk

https://cloud.google.com/compute/docs/disks/local-ssd#data_persistence

https://cloud.google.com/billing/docs/how-to/export-data-bigquery

https://cloud.google.com/resource-manager/docs/creating-managing-labels