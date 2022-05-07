# MultiCopy_Parallel_FEP_Simulations
# Interface to non-interacting multiple-copy namd script for FEP simulations

 running on HPC with runbatch_cuda (or runbatch) script:
 ./runbatch_cuda [configfile] [logfile] [total_num_nodes] +replicas [num_replicas] +stdout [logfile].%d
 total_num_nodes must be a multiple of num_replicas
 example: ./runbatch_cuda job0.conf job0.log 40 +replicas 20 +stdout job0.log.%d
