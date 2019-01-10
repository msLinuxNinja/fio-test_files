These files are used by FIO (Flexible IO Tester) to control IO testing. Each file runs a different test, each test will allocate four 4GB files to be used as IO targets. The files created are the same for each test so only a set of four files will be created in total.

All the tests bypass the pagecache to avoid false positives when doing IO, the idea of these tests is to verify disk performance.


# read-maxIOPS-random.fio 
This test runs RANDOM IO using 4K blocksize, with a smaller blocksize this test is suited for IOPS testing.
# read-maxIOPS-sequential.fio 	
This test runs SEQUENTIAL IO using 4K blocksize, with a smaller blocksize this test is suited for IOPS testing.
# read-maxTHROUGHPUT-random.fio 	
This test runs RANDOM IO using 1M Blocksize, a larger blocksize will yield higher throughput and lower IOPS.
# read-maxTHROUGHPUT-sequential.fio 	
This test runs SEQUENTIAL IO using 1M Blocksize, a larger blocksize will yield higher throughput and lower IOPS.
# rw-random-IOPS.fio 	
This test runs RANDOM reads and writes in a 50/50 ratio using 4K blocksize suited for IOPS testing.
# rw-random-THROUGHPUT.fio 	
This test runs RANDOM reads and writes in a 50/50 ratio using 1M blocksize yielding higher throughput and lower IOPS.
# write-maxIOPS-random.fio
This test runs RANDOM IO using 4K blocksize, with a smaller blocksize this test is suited for IOPS testing.
# write-maxIOPS-sequential.fio 	
This test runs SEQUENTIAL IO using 4K blocksize, with a smaller blocksize this test is suited for IOPS testing.
# write-maxTHROUGHPUT-random.fio 	
This test runs RANDOM IO using 1M Blocksize, a larger blocksize will yield higher throughput and lower IOPS.
# write-maxTHROUGHPUT-sequential.fio 	
This test runs SEQUENTIAL IO using 1M Blocksize, a larger blocksize will yield higher throughput and lower IOPS.
