# Comparing `tmp/reasonable-0.2.2a3.tar.gz` & `tmp/reasonable-0.2.2a4.tar.gz`

## Comparing `reasonable-0.2.2a3.tar` & `reasonable-0.2.2a4.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 reasonable-0.2.2a3/Cargo.toml
--rw-r--r--   0      501       20      111 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/.cargo/config
--rw-r--r--   0      501       20     6211 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/.github/workflows/Python.yml
--rw-r--r--   0      501       20     2263 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/.github/workflows/builds.yml
--rw-r--r--   0      501       20      542 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/.github/workflows/manylinux_build.sh
--rw-r--r--   0      501       20     1127 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/.github/workflows/nightly-builds.yml
--rw-r--r--   0      501       20      568 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/.gitignore
--rw-r--r--   0      501       20    17449 2022-11-20 00:00:56.000000 reasonable-0.2.2a3/Cargo.lock
--rw-r--r--   0      501       20     1519 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/LICENSE
--rw-r--r--   0      501       20     1608 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/Makefile
--rw-r--r--   0      501       20     5360 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/README.md
--rw-r--r--   0      501       20     4490 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/my_benchmark.rs
--rw-r--r--   0      501       20     3755 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/bench.py
--rw-r--r--   0      501       20   438888 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/ACAD(v1.1).ttl
--rw-r--r--   0      501       20    15738 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/AMRL(v1.1).ttl
--rw-r--r--   0      501       20     4663 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/AOB4(v1.1).ttl
--rw-r--r--   0      501       20     2456 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/AQUA(v1.1).ttl
--rw-r--r--   0      501       20   148837 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/ARC(v1.1).ttl
--rw-r--r--   0      501       20     8626 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/ART(v1.1).ttl
--rw-r--r--   0      501       20    32114 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/ARTX(v1.1).ttl
--rw-r--r--   0      501       20    32336 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/ASMUN(v1.1).ttl
--rw-r--r--   0      501       20     5821 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/BIXB(v1.1).ttl
--rw-r--r--   0      501       20   680383 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/BRIG(v1.1).ttl
--rw-r--r--   0      501       20    52446 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/BWFP(v1.1).ttl
--rw-r--r--   0      501       20   103849 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/Bainer(v1.1).ttl
--rw-r--r--   0      501       20     2740 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/C113(v1.1).ttl
--rw-r--r--   0      501       20   234090 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/CHEM(v1.1).ttl
--rw-r--r--   0      501       20   201232 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/CHEMX(v1.1).ttl
--rw-r--r--   0      501       20    26964 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/CONT(v1.1).ttl
--rw-r--r--   0      501       20    23617 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/COWL(v1.1).ttl
--rw-r--r--   0      501       20    56380 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/CRUS(v1.1).ttl
--rw-r--r--   0      501       20     2785 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/CURR(v1.1).ttl
--rw-r--r--   0      501       20   197473 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/DH(v1.1).ttl
--rw-r--r--   0      501       20   435076 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/EPS(v1.1).ttl
--rw-r--r--   0      501       20    27951 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/FDPD(v1.1).ttl
--rw-r--r--   0      501       20   530501 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/GBSF(v1.1).ttl
--rw-r--r--   0      501       20   210071 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/GHA_ICS(v1.1).ttl
--rw-r--r--   0      501       20    48299 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/GIEDT(v1.1).ttl
--rw-r--r--   0      501       20     5808 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/GILM(v1.1).ttl
--rw-r--r--   0      501       20   304349 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/HART(v1.1).ttl
--rw-r--r--   0      501       20     8128 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/HICK(v1.1).ttl
--rw-r--r--   0      501       20     5628 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/HUNT(v1.1).ttl
--rw-r--r--   0      501       20   303396 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/HUTCH(v1.1).ttl
--rw-r--r--   0      501       20   194712 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/HWC(v1.1).ttl
--rw-r--r--   0      501       20    57424 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/JUNGER(v1.1).ttl
--rw-r--r--   0      501       20     6215 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/KERR(v1.1).ttl
--rw-r--r--   0      501       20     6999 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/KING(v1.1).ttl
--rw-r--r--   0      501       20     6609 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/KLEIBER(v1.1).ttl
--rw-r--r--   0      501       20    18419 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/LFH(v1.1).ttl
--rw-r--r--   0      501       20    19160 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/LSA(v1.1).ttl
--rw-r--r--   0      501       20    84768 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/MADDY(v1.1).ttl
--rw-r--r--   0      501       20    28687 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/MANN(v1.1).ttl
--rw-r--r--   0      501       20    15662 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/MATH(v1.1).ttl
--rw-r--r--   0      501       20   131812 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/MEYR(v1.1).ttl
--rw-r--r--   0      501       20    23894 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/MIWF(v1.1).ttl
--rw-r--r--   0      501       20   164159 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/MRAK(v1.1).ttl
--rw-r--r--   0      501       20    18750 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/MSB(v1.1).ttl
--rw-r--r--   0      501       20    11894 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/MSC(v1.1).ttl
--rw-r--r--   0      501       20     3115 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/MSD(v1.1).ttl
--rw-r--r--   0      501       20    42466 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/MU(v1.1).ttl
--rw-r--r--   0      501       20     8421 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/MUSIC(v1.1).ttl
--rw-r--r--   0      501       20    14105 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/OLS(v1.1).ttl
--rw-r--r--   0      501       20   476097 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/PES_ICS(v1.1).ttl
--rw-r--r--   0      501       20     7860 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/PHSL(v1.1).ttl
--rw-r--r--   0      501       20     2785 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/PINE(v1.1).ttl
--rw-r--r--   0      501       20    86053 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/PRB(v1.1).ttl
--rw-r--r--   0      501       20    20839 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/RECH(v1.1).ttl
--rw-r--r--   0      501       20    42143 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/ROES(v1.1).ttl
--rw-r--r--   0      501       20     2454 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/RPL(v1.1).ttl
--rw-r--r--   0      501       20     5498 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/RYER(v1.1).ttl
--rw-r--r--   0      501       20    47682 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/SCC(v1.1).ttl
--rw-r--r--   0      501       20     6683 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/SCHM(v1.1).ttl
--rw-r--r--   0      501       20     2785 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/SEQU(v1.1).ttl
--rw-r--r--   0      501       20   271074 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/SHIELDS(v1.1).ttl
--rw-r--r--   0      501       20   166666 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/SLAB(v1.1).ttl
--rw-r--r--   0      501       20     6312 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/SLEC(v1.1).ttl
--rw-r--r--   0      501       20    63381 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/SMOA(v1.1).ttl
--rw-r--r--   0      501       20   489384 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/SOCS(v1.1).ttl
--rw-r--r--   0      501       20     4380 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/SPRL(v1.1).ttl
--rw-r--r--   0      501       20   222603 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/STOR(v1.1).ttl
--rw-r--r--   0      501       20    32752 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/SURGE3(v1.1).ttl
--rw-r--r--   0      501       20     3657 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/SWL(v1.1).ttl
--rw-r--r--   0      501       20    73442 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/TAPS(v1.1).ttl
--rw-r--r--   0      501       20     2457 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/THOR(v1.1).ttl
--rw-r--r--   0      501       20    91770 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/THUR(v1.1).ttl
--rw-r--r--   0      501       20    26122 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/TUPP(v1.1).ttl
--rw-r--r--   0      501       20    34129 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/VEIH(v1.1).ttl
--rw-r--r--   0      501       20   137513 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/VM2(v1.1).ttl
--rw-r--r--   0      501       20  1100244 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/VM3A(v1.1).ttl
--rw-r--r--   0      501       20     6920 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/VM3B(v1.1).ttl
--rw-r--r--   0      501       20    37918 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/VMEP(v1.1).ttl
--rw-r--r--   0      501       20   130411 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/VMIF(v1.1).ttl
--rw-r--r--   0      501       20    13294 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/VMLF(v1.1).ttl
--rw-r--r--   0      501       20    55576 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/VMTH(v1.1).ttl
--rw-r--r--   0      501       20     4286 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/VMTHB(v1.1).ttl
--rw-r--r--   0      501       20     4286 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/VMTHC(v1.1).ttl
--rw-r--r--   0      501       20    91018 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/WELL(v1.1).ttl
--rw-r--r--   0      501       20    27797 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/WICK(v1.1).ttl
--rw-r--r--   0      501       20    73670 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/WSRC(v1.1).ttl
--rw-r--r--   0      501       20    23245 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/YOUNG(v1.1).ttl
--rw-r--r--   0      501       20    13281 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/avenal-animal-shelter(v1.1).ttl
--rw-r--r--   0      501       20    39438 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/avenal-movie-theatre(v1.1).ttl
--rw-r--r--   0      501       20    10692 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/avenal-public-works-yard(v1.1).ttl
--rw-r--r--   0      501       20    14596 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/avenal-recreation-center(v1.1).ttl
--rw-r--r--   0      501       20    27336 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/avenal-veterans-hall(v1.1).ttl
--rw-r--r--   0      501       20    29969 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl
--rw-r--r--   0      501       20    82637 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/ciee(v1.1).ttl
--rw-r--r--   0      501       20    81292 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl
--rw-r--r--   0      501       20   474074 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/csu-dominguez-hills(v1.1).ttl
--rw-r--r--   0      501       20    13557 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/garber(v1.1).ttl
--rw-r--r--   0      501       20    24179 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/hayward-station-1(v1.1).ttl
--rw-r--r--   0      501       20    18716 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/hayward-station-8(v1.1).ttl
--rw-r--r--   0      501       20    76388 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/jesse-turner-center(v1.1).ttl
--rw-r--r--   0      501       20    10088 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/local-butcher-shop(v1.1).ttl
--rw-r--r--   0      501       20    21969 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl
--rw-r--r--   0      501       20    58913 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/orinda-community-center(v1.1).ttl
--rw-r--r--   0      501       20    98730 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/orinda-public-library(v1.1).ttl
--rw-r--r--   0      501       20    18839 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/rfs(v1.1).ttl
--rw-r--r--   0      501       20   424960 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/sdh(v1.1).ttl
--rw-r--r--   0      501       20    31717 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl
--rw-r--r--   0      501       20    32735 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/buildings/word-of-faith-cc(v1.1).ttl
--rw-r--r--   0      501       20       41 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/benches/python/requirements.txt
--rw-r--r--   0      501       20  2189973 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/example_models/ontologies/Brick.n3
--rw-r--r--   0      501       20    64515 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/example_models/ontologies/owl.n3
--rw-r--r--   0      501       20     3812 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/example_models/ontologies/rdfs.ttl
--rw-r--r--   0      501       20     2263 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/example_models/small1.n3
--rw-r--r--   0      501       20   707359 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/example_models/soda_hall.n3
--rw-r--r--   0      501       20    43207 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/img/benchmark.png
--rw-r--r--   0      501       20    21469 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/poetry.lock
--rw-r--r--   0      501       20      599 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/pyproject.toml
--rw-r--r--   0      501       20       84 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/reasonable/__init__.py
--rwxr-xr-x   0      501       20     1117 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/scripts/bench_examples.sh
--rwxr-xr-x   0      501       20      318 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/scripts/convert_to_n3.py
--rwxr-xr-x   0      501       20      323 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/scripts/reason_owlrl.py
--rw-r--r--   0      501       20     5741 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/src/common.rs
--rw-r--r--   0      501       20     4181 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/src/disjoint_sets.rs
--rw-r--r--   0      501       20     2102 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/src/error.rs
--rw-r--r--   0      501       20     1034 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/src/index.rs
--rw-r--r--   0      501       20      795 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/src/lib.rs
--rw-r--r--   0      501       20      584 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/src/main.rs
--rw-r--r--   0      501       20     6253 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/src/pyreason.rs
--rw-r--r--   0      501       20    11950 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/src/query.rs
--rw-r--r--   0      501       20    61875 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/src/reasoner.rs
--rw-r--r--   0      501       20    26068 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/src/tests.rs
--rw-r--r--   0      501       20      350 2022-11-19 23:59:05.000000 reasonable-0.2.2a3/test.py
--rw-r--r--   0        0        0     5733 1970-01-01 00:00:00.000000 reasonable-0.2.2a3/PKG-INFO
+-rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 reasonable-0.2.2a4/Cargo.toml
+-rw-r--r--   0      501       20      111 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.cargo/config
+-rw-r--r--   0      501       20     7144 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.github/workflows/Python.yml
+-rw-r--r--   0      501       20     2263 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.github/workflows/builds.yml
+-rw-r--r--   0      501       20      542 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.github/workflows/manylinux_build.sh
+-rw-r--r--   0      501       20     1127 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.github/workflows/nightly-builds.yml
+-rw-r--r--   0      501       20      568 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.gitignore
+-rw-r--r--   0      501       20    17449 2022-11-26 19:12:43.000000 reasonable-0.2.2a4/Cargo.lock
+-rw-r--r--   0      501       20     1519 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/LICENSE
+-rw-r--r--   0      501       20     1608 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/Makefile
+-rw-r--r--   0      501       20     5360 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/README.md
+-rw-r--r--   0      501       20     4490 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/my_benchmark.rs
+-rw-r--r--   0      501       20     3755 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/bench.py
+-rw-r--r--   0      501       20   438888 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ACAD(v1.1).ttl
+-rw-r--r--   0      501       20    15738 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/AMRL(v1.1).ttl
+-rw-r--r--   0      501       20     4663 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/AOB4(v1.1).ttl
+-rw-r--r--   0      501       20     2456 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/AQUA(v1.1).ttl
+-rw-r--r--   0      501       20   148837 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ARC(v1.1).ttl
+-rw-r--r--   0      501       20     8626 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ART(v1.1).ttl
+-rw-r--r--   0      501       20    32114 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ARTX(v1.1).ttl
+-rw-r--r--   0      501       20    32336 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ASMUN(v1.1).ttl
+-rw-r--r--   0      501       20     5821 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/BIXB(v1.1).ttl
+-rw-r--r--   0      501       20   680383 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/BRIG(v1.1).ttl
+-rw-r--r--   0      501       20    52446 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/BWFP(v1.1).ttl
+-rw-r--r--   0      501       20   103849 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/Bainer(v1.1).ttl
+-rw-r--r--   0      501       20     2740 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/C113(v1.1).ttl
+-rw-r--r--   0      501       20   234090 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/CHEM(v1.1).ttl
+-rw-r--r--   0      501       20   201232 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/CHEMX(v1.1).ttl
+-rw-r--r--   0      501       20    26964 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/CONT(v1.1).ttl
+-rw-r--r--   0      501       20    23617 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/COWL(v1.1).ttl
+-rw-r--r--   0      501       20    56380 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/CRUS(v1.1).ttl
+-rw-r--r--   0      501       20     2785 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/CURR(v1.1).ttl
+-rw-r--r--   0      501       20   197473 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/DH(v1.1).ttl
+-rw-r--r--   0      501       20   435076 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/EPS(v1.1).ttl
+-rw-r--r--   0      501       20    27951 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/FDPD(v1.1).ttl
+-rw-r--r--   0      501       20   530501 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/GBSF(v1.1).ttl
+-rw-r--r--   0      501       20   210071 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/GHA_ICS(v1.1).ttl
+-rw-r--r--   0      501       20    48299 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/GIEDT(v1.1).ttl
+-rw-r--r--   0      501       20     5808 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/GILM(v1.1).ttl
+-rw-r--r--   0      501       20   304349 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/HART(v1.1).ttl
+-rw-r--r--   0      501       20     8128 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/HICK(v1.1).ttl
+-rw-r--r--   0      501       20     5628 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/HUNT(v1.1).ttl
+-rw-r--r--   0      501       20   303396 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/HUTCH(v1.1).ttl
+-rw-r--r--   0      501       20   194712 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/HWC(v1.1).ttl
+-rw-r--r--   0      501       20    57424 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/JUNGER(v1.1).ttl
+-rw-r--r--   0      501       20     6215 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/KERR(v1.1).ttl
+-rw-r--r--   0      501       20     6999 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/KING(v1.1).ttl
+-rw-r--r--   0      501       20     6609 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/KLEIBER(v1.1).ttl
+-rw-r--r--   0      501       20    18419 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/LFH(v1.1).ttl
+-rw-r--r--   0      501       20    19160 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/LSA(v1.1).ttl
+-rw-r--r--   0      501       20    84768 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MADDY(v1.1).ttl
+-rw-r--r--   0      501       20    28687 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MANN(v1.1).ttl
+-rw-r--r--   0      501       20    15662 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MATH(v1.1).ttl
+-rw-r--r--   0      501       20   131812 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MEYR(v1.1).ttl
+-rw-r--r--   0      501       20    23894 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MIWF(v1.1).ttl
+-rw-r--r--   0      501       20   164159 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MRAK(v1.1).ttl
+-rw-r--r--   0      501       20    18750 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MSB(v1.1).ttl
+-rw-r--r--   0      501       20    11894 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MSC(v1.1).ttl
+-rw-r--r--   0      501       20     3115 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MSD(v1.1).ttl
+-rw-r--r--   0      501       20    42466 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MU(v1.1).ttl
+-rw-r--r--   0      501       20     8421 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MUSIC(v1.1).ttl
+-rw-r--r--   0      501       20    14105 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/OLS(v1.1).ttl
+-rw-r--r--   0      501       20   476097 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/PES_ICS(v1.1).ttl
+-rw-r--r--   0      501       20     7860 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/PHSL(v1.1).ttl
+-rw-r--r--   0      501       20     2785 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/PINE(v1.1).ttl
+-rw-r--r--   0      501       20    86053 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/PRB(v1.1).ttl
+-rw-r--r--   0      501       20    20839 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/RECH(v1.1).ttl
+-rw-r--r--   0      501       20    42143 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ROES(v1.1).ttl
+-rw-r--r--   0      501       20     2454 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/RPL(v1.1).ttl
+-rw-r--r--   0      501       20     5498 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/RYER(v1.1).ttl
+-rw-r--r--   0      501       20    47682 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SCC(v1.1).ttl
+-rw-r--r--   0      501       20     6683 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SCHM(v1.1).ttl
+-rw-r--r--   0      501       20     2785 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SEQU(v1.1).ttl
+-rw-r--r--   0      501       20   271074 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SHIELDS(v1.1).ttl
+-rw-r--r--   0      501       20   166666 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SLAB(v1.1).ttl
+-rw-r--r--   0      501       20     6312 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SLEC(v1.1).ttl
+-rw-r--r--   0      501       20    63381 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SMOA(v1.1).ttl
+-rw-r--r--   0      501       20   489384 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SOCS(v1.1).ttl
+-rw-r--r--   0      501       20     4380 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SPRL(v1.1).ttl
+-rw-r--r--   0      501       20   222603 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/STOR(v1.1).ttl
+-rw-r--r--   0      501       20    32752 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SURGE3(v1.1).ttl
+-rw-r--r--   0      501       20     3657 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SWL(v1.1).ttl
+-rw-r--r--   0      501       20    73442 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/TAPS(v1.1).ttl
+-rw-r--r--   0      501       20     2457 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/THOR(v1.1).ttl
+-rw-r--r--   0      501       20    91770 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/THUR(v1.1).ttl
+-rw-r--r--   0      501       20    26122 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/TUPP(v1.1).ttl
+-rw-r--r--   0      501       20    34129 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VEIH(v1.1).ttl
+-rw-r--r--   0      501       20   137513 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VM2(v1.1).ttl
+-rw-r--r--   0      501       20  1100244 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VM3A(v1.1).ttl
+-rw-r--r--   0      501       20     6920 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VM3B(v1.1).ttl
+-rw-r--r--   0      501       20    37918 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMEP(v1.1).ttl
+-rw-r--r--   0      501       20   130411 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMIF(v1.1).ttl
+-rw-r--r--   0      501       20    13294 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMLF(v1.1).ttl
+-rw-r--r--   0      501       20    55576 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMTH(v1.1).ttl
+-rw-r--r--   0      501       20     4286 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMTHB(v1.1).ttl
+-rw-r--r--   0      501       20     4286 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMTHC(v1.1).ttl
+-rw-r--r--   0      501       20    91018 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/WELL(v1.1).ttl
+-rw-r--r--   0      501       20    27797 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/WICK(v1.1).ttl
+-rw-r--r--   0      501       20    73670 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/WSRC(v1.1).ttl
+-rw-r--r--   0      501       20    23245 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/YOUNG(v1.1).ttl
+-rw-r--r--   0      501       20    13281 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/avenal-animal-shelter(v1.1).ttl
+-rw-r--r--   0      501       20    39438 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/avenal-movie-theatre(v1.1).ttl
+-rw-r--r--   0      501       20    10692 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/avenal-public-works-yard(v1.1).ttl
+-rw-r--r--   0      501       20    14596 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/avenal-recreation-center(v1.1).ttl
+-rw-r--r--   0      501       20    27336 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/avenal-veterans-hall(v1.1).ttl
+-rw-r--r--   0      501       20    29969 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl
+-rw-r--r--   0      501       20    82637 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ciee(v1.1).ttl
+-rw-r--r--   0      501       20    81292 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl
+-rw-r--r--   0      501       20   474074 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/csu-dominguez-hills(v1.1).ttl
+-rw-r--r--   0      501       20    13557 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/garber(v1.1).ttl
+-rw-r--r--   0      501       20    24179 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/hayward-station-1(v1.1).ttl
+-rw-r--r--   0      501       20    18716 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/hayward-station-8(v1.1).ttl
+-rw-r--r--   0      501       20    76388 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/jesse-turner-center(v1.1).ttl
+-rw-r--r--   0      501       20    10088 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/local-butcher-shop(v1.1).ttl
+-rw-r--r--   0      501       20    21969 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl
+-rw-r--r--   0      501       20    58913 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/orinda-community-center(v1.1).ttl
+-rw-r--r--   0      501       20    98730 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/orinda-public-library(v1.1).ttl
+-rw-r--r--   0      501       20    18839 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/rfs(v1.1).ttl
+-rw-r--r--   0      501       20   424960 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/sdh(v1.1).ttl
+-rw-r--r--   0      501       20    31717 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl
+-rw-r--r--   0      501       20    32735 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/word-of-faith-cc(v1.1).ttl
+-rw-r--r--   0      501       20       41 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/requirements.txt
+-rw-r--r--   0      501       20  2189973 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/example_models/ontologies/Brick.n3
+-rw-r--r--   0      501       20    64515 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/example_models/ontologies/owl.n3
+-rw-r--r--   0      501       20     3812 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/example_models/ontologies/rdfs.ttl
+-rw-r--r--   0      501       20     2263 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/example_models/small1.n3
+-rw-r--r--   0      501       20   707359 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/example_models/soda_hall.n3
+-rw-r--r--   0      501       20    43207 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/img/benchmark.png
+-rw-r--r--   0      501       20    21469 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/poetry.lock
+-rw-r--r--   0      501       20      599 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/pyproject.toml
+-rw-r--r--   0      501       20       84 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/reasonable/__init__.py
+-rwxr-xr-x   0      501       20     1117 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/scripts/bench_examples.sh
+-rwxr-xr-x   0      501       20      318 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/scripts/convert_to_n3.py
+-rwxr-xr-x   0      501       20      323 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/scripts/reason_owlrl.py
+-rw-r--r--   0      501       20     5741 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/common.rs
+-rw-r--r--   0      501       20     4181 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/disjoint_sets.rs
+-rw-r--r--   0      501       20     2102 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/error.rs
+-rw-r--r--   0      501       20     1034 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/index.rs
+-rw-r--r--   0      501       20      795 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/lib.rs
+-rw-r--r--   0      501       20      584 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/main.rs
+-rw-r--r--   0      501       20     6240 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/pyreason.rs
+-rw-r--r--   0      501       20    11950 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/query.rs
+-rw-r--r--   0      501       20    61875 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/reasoner.rs
+-rw-r--r--   0      501       20    26068 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/tests.rs
+-rw-r--r--   0      501       20      350 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/test.py
+-rw-r--r--   0        0        0     5733 1970-01-01 00:00:00.000000 reasonable-0.2.2a4/PKG-INFO
```

### Comparing `reasonable-0.2.2a3/Cargo.toml` & `reasonable-0.2.2a4/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "reasonable"
-version = "0.2.2-a3"
+version = "0.2.2-a4"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 repository = "https://github.com/gtfierro/reasonable"
 homepage = "https://brickschema.org/"
 license-file = "LICENSE"
 readme = "README.md"
 description = "An OWL 2 RL reasoner with reasonable performance"
 edition = "2018"
```

### Comparing `reasonable-0.2.2a3/.github/workflows/Python.yml` & `reasonable-0.2.2a4/.github/workflows/Python.yml`

 * *Files 4% similar despite different names*

```diff
@@ -187,14 +187,40 @@
           #      python3 -c "import reasonable"
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
+  debian:
+    name: Debian package
+    runs-on: ubuntu-latest
+    needs: [ macos, windows, linux, linux-cross]
+    steps:
+      - uses: actions/download-artifact@v3
+        with:
+          name: wheels
+      - uses: actions/setup-python@v4
+        with:
+          python-version: '3.10'
+      - name: Install deps
+        run: sudo apt install apt-file dpkg-dev fakeroot build-essential devscripts debhelper binutils-arm-linux-gnueabihf
+      - name: apt-file update
+        run: sudo apt-file update
+      - run: python3 -m pip install wheel2deb
+        name: install wheel2deb
+      - run: find . -name '*linux*' -exec basename {} \; | xargs wheel2deb -v --map attrs=attr -i
+        name: convert wheels to deb source packages
+      - run: wheel2deb -v build
+        name: build .deb
+      - run: dpkg -i output/*.deb
+        name: install built packages
+      - run: python3 -c "import reasonable"
+        name: test instalation
+
   release:
     name: Release
     runs-on: ubuntu-latest
       #if: "startsWith(github.ref, 'refs/tags/')"
     needs: [ macos, windows, linux, linux-cross]
       #, linux-cross, musllinux, musllinux-cross ]
     steps:
```

### Comparing `reasonable-0.2.2a3/.github/workflows/builds.yml` & `reasonable-0.2.2a4/.github/workflows/builds.yml`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/.github/workflows/manylinux_build.sh` & `reasonable-0.2.2a4/.github/workflows/manylinux_build.sh`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/.github/workflows/nightly-builds.yml` & `reasonable-0.2.2a4/.github/workflows/nightly-builds.yml`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/.gitignore` & `reasonable-0.2.2a4/.gitignore`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/Cargo.lock` & `reasonable-0.2.2a4/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.19"
+version = "0.7.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4f55bd91a0978cbfd91c457a164bab8b4001c833b7f323132c0a4e1922dd44e"
+checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
 version = "1.0.66"
@@ -385,15 +385,15 @@
 name = "rdf"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb1725bf0133fe4a3279e18efd6d69f952cb8356bf8b835023042e1b98d4c646"
 
 [[package]]
 name = "reasonable"
-version = "0.2.2-a3"
+version = "0.2.2-a4"
 dependencies = [
  "anyhow",
  "datafrog",
  "disjoint-sets",
  "env_logger",
  "farmhash",
  "itertools",
@@ -490,17 +490,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.88"
+version = "1.0.89"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e8b3801309262e8184d9687fb697586833e939767aea0dda89f5a8e650e8bd7"
+checksum = "020ff22c755c2ed3f8cf162dbb41a7268d934702f3ed3631656ea597e08fc3db"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
```

### Comparing `reasonable-0.2.2a3/LICENSE` & `reasonable-0.2.2a4/LICENSE`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/Makefile` & `reasonable-0.2.2a4/Makefile`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/README.md` & `reasonable-0.2.2a4/README.md`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/my_benchmark.rs` & `reasonable-0.2.2a4/benches/my_benchmark.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/bench.py` & `reasonable-0.2.2a4/benches/python/bench.py`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/ACAD(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/ACAD(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/AMRL(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/AMRL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/AOB4(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/AOB4(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/AQUA(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/AQUA(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/ARC(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/ARC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/ART(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/ART(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/ARTX(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/ARTX(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/ASMUN(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/ASMUN(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/BIXB(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/BIXB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/BRIG(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/BRIG(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/BWFP(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/BWFP(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/Bainer(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/Bainer(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/C113(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/C113(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/CHEM(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/CHEM(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/CHEMX(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/CHEMX(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/CONT(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/CONT(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/COWL(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/COWL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/CRUS(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/CRUS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/CURR(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/CURR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/DH(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/DH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/EPS(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/EPS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/FDPD(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/FDPD(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/GBSF(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/GBSF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/GHA_ICS(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/GHA_ICS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/GIEDT(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/GIEDT(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/GILM(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/GILM(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/HART(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/HART(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/HICK(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/HICK(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/HUNT(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/HUNT(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/HUTCH(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/HUTCH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/HWC(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/HWC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/JUNGER(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/JUNGER(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/KERR(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/KERR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/KING(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/KING(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/KLEIBER(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/KLEIBER(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/LFH(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/LFH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/LSA(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/LSA(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/MADDY(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/MADDY(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/MANN(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/MANN(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/MATH(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/MATH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/MEYR(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/MEYR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/MIWF(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/MIWF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/MRAK(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/MRAK(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/MSB(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/MSB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/MSC(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/MSC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/MSD(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/MSD(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/MU(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/MU(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/MUSIC(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/MUSIC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/OLS(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/OLS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/PES_ICS(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/PES_ICS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/PHSL(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/PHSL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/PINE(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/PINE(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/PRB(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/PRB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/RECH(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/RECH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/ROES(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/ROES(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/RPL(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/RPL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/RYER(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/RYER(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/SCC(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/SCC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/SCHM(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/SCHM(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/SEQU(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/SEQU(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/SHIELDS(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/SHIELDS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/SLAB(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/SLAB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/SLEC(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/SLEC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/SMOA(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/SMOA(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/SOCS(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/SOCS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/SPRL(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/SPRL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/STOR(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/STOR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/SURGE3(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/SURGE3(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/SWL(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/SWL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/TAPS(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/TAPS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/THOR(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/THOR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/THUR(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/THUR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/TUPP(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/TUPP(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/VEIH(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/VEIH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/VM2(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/VM2(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/VM3A(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/VM3A(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/VM3B(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/VM3B(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/VMEP(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/VMEP(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/VMIF(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/VMIF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/VMLF(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/VMLF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/VMTH(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/VMTH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/VMTHB(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/VMTHB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/VMTHC(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/VMTHC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/WELL(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/WELL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/WICK(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/WICK(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/WSRC(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/WSRC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/YOUNG(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/YOUNG(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/avenal-animal-shelter(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/avenal-animal-shelter(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/avenal-movie-theatre(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/avenal-movie-theatre(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/avenal-public-works-yard(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/avenal-public-works-yard(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/avenal-recreation-center(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/avenal-recreation-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/avenal-veterans-hall(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/avenal-veterans-hall(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/ciee(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/ciee(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/csu-dominguez-hills(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/csu-dominguez-hills(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/garber(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/garber(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/hayward-station-1(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/hayward-station-1(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/hayward-station-8(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/hayward-station-8(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/jesse-turner-center(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/jesse-turner-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/local-butcher-shop(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/local-butcher-shop(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/orinda-community-center(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/orinda-community-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/orinda-public-library(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/orinda-public-library(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/rfs(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/rfs(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/sdh(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/sdh(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/benches/python/buildings/word-of-faith-cc(v1.1).ttl` & `reasonable-0.2.2a4/benches/python/buildings/word-of-faith-cc(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/example_models/ontologies/Brick.n3` & `reasonable-0.2.2a4/example_models/ontologies/Brick.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/example_models/ontologies/owl.n3` & `reasonable-0.2.2a4/example_models/ontologies/owl.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/example_models/ontologies/rdfs.ttl` & `reasonable-0.2.2a4/example_models/ontologies/rdfs.ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/example_models/small1.n3` & `reasonable-0.2.2a4/example_models/small1.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/example_models/soda_hall.n3` & `reasonable-0.2.2a4/example_models/soda_hall.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/img/benchmark.png` & `reasonable-0.2.2a4/img/benchmark.png`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/poetry.lock` & `reasonable-0.2.2a4/poetry.lock`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/pyproject.toml` & `reasonable-0.2.2a4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasonable"
-version = "0.2.2a3"
+version = "0.2.2a4"
 description = "Python interface to 'reasonable', a Datalog implementation of the OWL 2 RL profile"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "bsd-3-clause"
 readme = "README.md"
 homepage = "https://github.com/gtfierro/reasonable"
 
 [tool.poetry.dependencies]
```

### Comparing `reasonable-0.2.2a3/scripts/bench_examples.sh` & `reasonable-0.2.2a4/scripts/bench_examples.sh`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/src/common.rs` & `reasonable-0.2.2a4/src/common.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/src/disjoint_sets.rs` & `reasonable-0.2.2a4/src/disjoint_sets.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/src/error.rs` & `reasonable-0.2.2a4/src/error.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/src/index.rs` & `reasonable-0.2.2a4/src/index.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/src/lib.rs` & `reasonable-0.2.2a4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/src/main.rs` & `reasonable-0.2.2a4/src/main.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/src/pyreason.rs` & `reasonable-0.2.2a4/src/pyreason.rs`

 * *Files 1% similar despite different names*

```diff
@@ -147,18 +147,17 @@
 
     /// Loads in triples from an RDFlib Graph or any other object that can be converted into a list
     /// of triples (length-3 tuples of URI-formatted strings)
     pub fn from_graph(&mut self, graph: PyObject) -> PyResult<()> {
         Python::with_gil(|py| {
             let converters = PyModule::from_code(
                 py,
-                "
-    def get_triples(graph):
-        return list(graph)
-    ",
+                "def get_triples(graph):
+    return list(graph)
+",
                 "converters.pg",
                 "converters",
             )?;
             let l: &PyList = converters
                 .getattr("get_triples")?
                 .call1((graph,))?
                 .downcast()?;
```

### Comparing `reasonable-0.2.2a3/src/query.rs` & `reasonable-0.2.2a4/src/query.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/src/reasoner.rs` & `reasonable-0.2.2a4/src/reasoner.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/src/tests.rs` & `reasonable-0.2.2a4/src/tests.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a3/PKG-INFO` & `reasonable-0.2.2a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasonable
-Version: 0.2.2a3
+Version: 0.2.2a4
 Summary: An OWL 2 RL reasoner with reasonable performance
 Home-Page: https://brickschema.org/
 Author: Gabe Fierro <gtfierro@mines.edu>
 Author-email: Gabe Fierro <gtfierro@mines.edu>
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/gtfierro/reasonable
```

