*Modified code:
1. xfs/libxfs/xfs_ialloc.c:1701-1708: Change AG selection policy.
2.  Various places between /* JACOB MOD BELOW */  and /* JACOB MOD ABOVE */ : For code tracing.

*Step to compile:
cd ~/rpmbuild/BUILD/kernel-4.2.fc23/linux-4.2.5-300.fc23.x86_64/make modules SUBDIRS=fs/xfs
The kernel module is located at ~/rpmbuild/BUILD/kernel-4.2.fc23/linux-4.2.5-300.fc23.x86_64/fs/xfs/xfs.ko

*Step to load modified kernel module:
Assume our new kernel module is placed at home directory.
rmmod xfs # unload XFS module, if any is loaded
insmod xfs.ko
