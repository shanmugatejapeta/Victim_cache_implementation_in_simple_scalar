# Victim_cache_implementation_in_simple_scalar
A victim cache is a small fully associative buffer between L1 and main memory that stores recently evicted blocks to reduce conflict misses. On an L1 miss, it checks the victim cache; if found, the block is swapped back to L1, improving hit rate and performance without increasing cache associativity.

Steps to run:
replace the sim-cache.c file in your simple-scaler
make clean
make
./sim-cache -victim:entries 0 -cache:dl1 dl1:128:32:1:l -cache:dl2 ul2:1024:64:4:l ../Labs/Pisa/anagram
