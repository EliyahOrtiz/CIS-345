xv6 getprocs System Call

Files modified:
modified:   Makefile
new file:   getprocs.patch
modified:   kernel/syscall.c
modified:   kernel/syscall.h
modified:   kernel/sysproc.c
new file:   user/getprocs.c
modified:   user/user.h
modified:   user/usys.pl

Syscall number chosen: 23

sys_ getprocs loops over proc[NPROC] and counts all the processes that are UNUSED and returns the count.

Example Output:\

$ getprocs
Processes running: 1034
