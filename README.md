# run-next-job
Run a job after previous slurm jobs are finished

This script checks a slurm queue for a list of jobIDs and launches a
command, when the jobs are finished.

## Usage: 
run_next_job.sh -j <JobId> -n <next command> [-i <interval> -d]

### required:
-j    JobID: Comma separated list of Job IDs to check  
-n    next command: Command that should be run next (write in '' and set executable)  

### optional:
-i    interval: Time between each check. Use number and suffix (s,m,h,d)  
                default:10m  
-d:   Debug Mode  
-h    display help  
