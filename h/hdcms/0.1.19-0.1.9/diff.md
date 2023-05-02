# Comparing `tmp/hdcms-0.1.19.tar.gz` & `tmp/hdcms-0.1.9.tar.gz`

## Comparing `hdcms-0.1.19.tar` & `hdcms-0.1.9.tar`

### file list

```diff
@@ -1,1535 +1,16 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 hdcms-0.1.19/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/.DS_Store
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/README.md
--rw-r--r--   0        0        0    82220 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/paper_example_1.ipynb
--rw-r--r--   0        0        0   656886 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/paper_example_2.ipynb
--rw-r--r--   0        0        0   529138 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/paper_visualization.ipynb
--rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/start_here.ipynb
--rw-r--r--   0        0        0    59948 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/tmp.png
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/.DS_Store
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/ex1.txt
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/ex2.txt
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/ex3.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/ex4.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/ex5.txt
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/ex6.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/ex7.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/.DS_Store
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/01-01.txt
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/01-02.txt
--rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/01-03.txt
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/01-04.txt
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/01-05.txt
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/01-06.txt
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/01-07.txt
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/01-08.txt
--rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/01-09.txt
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/01-10.txt
--rw-r--r--   0        0        0    10322 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/02-01.txt
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/02-02.txt
--rw-r--r--   0        0        0    10285 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/02-03.txt
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/02-04.txt
--rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/02-05.txt
--rw-r--r--   0        0        0    10329 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/02-06.txt
--rw-r--r--   0        0        0    10543 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/02-07.txt
--rw-r--r--   0        0        0    10152 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/02-08.txt
--rw-r--r--   0        0        0    11058 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/02-09.txt
--rw-r--r--   0        0        0    10526 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/02-10.txt
--rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/03-01.txt
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/03-02.txt
--rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/03-03.txt
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/03-04.txt
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/03-05.txt
--rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/03-06.txt
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/03-07.txt
--rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/03-08.txt
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/03-09.txt
--rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/03-10.txt
--rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/04-01.txt
--rw-r--r--   0        0        0     8866 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/04-02.txt
--rw-r--r--   0        0        0     8547 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/04-03.txt
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/04-04.txt
--rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/04-05.txt
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/04-06.txt
--rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/04-07.txt
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/04-08.txt
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/04-09.txt
--rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/04-10.txt
--rw-r--r--   0        0        0     6566 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/05-01.txt
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/05-02.txt
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/05-03.txt
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/05-04.txt
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/05-05.txt
--rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/05-06.txt
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/05-07.txt
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/05-08.txt
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/05-09.txt
--rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/05-10.txt
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/06-01.txt
--rw-r--r--   0        0        0     6566 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/06-02.txt
--rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/06-03.txt
--rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/06-04.txt
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/06-05.txt
--rw-r--r--   0        0        0     6085 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/06-06.txt
--rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/06-07.txt
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/06-08.txt
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/06-09.txt
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/06-10.txt
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/07-01.txt
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/07-02.txt
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/07-03.txt
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/07-04.txt
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/07-05.txt
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/07-06.txt
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/07-07.txt
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/07-08.txt
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/07-09.txt
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/07-10.txt
--rw-r--r--   0        0        0    11249 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/08-01.txt
--rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/08-02.txt
--rw-r--r--   0        0        0    11188 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/08-03.txt
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/08-04.txt
--rw-r--r--   0        0        0    12415 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/08-05.txt
--rw-r--r--   0        0        0    11051 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/08-06.txt
--rw-r--r--   0        0        0    10953 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/08-07.txt
--rw-r--r--   0        0        0    11094 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/08-08.txt
--rw-r--r--   0        0        0    11096 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/08-09.txt
--rw-r--r--   0        0        0    11317 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/08-10.txt
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/09-01.txt
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/09-02.txt
--rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/09-03.txt
--rw-r--r--   0        0        0     7426 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/09-04.txt
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/09-05.txt
--rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/09-06.txt
--rw-r--r--   0        0        0     7528 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/09-07.txt
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/09-08.txt
--rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/09-09.txt
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/09-10.txt
--rw-r--r--   0        0        0     6833 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/10-01.txt
--rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/10-02.txt
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/10-03.txt
--rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/10-04.txt
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/10-05.txt
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/10-06.txt
--rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/10-07.txt
--rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/10-08.txt
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/10-09.txt
--rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/10-10.txt
--rw-r--r--   0        0        0    10626 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/11-01.txt
--rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/11-02.txt
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/11-03.txt
--rw-r--r--   0        0        0    10562 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/11-04.txt
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/11-05.txt
--rw-r--r--   0        0        0    10673 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/11-06.txt
--rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/11-07.txt
--rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/11-08.txt
--rw-r--r--   0        0        0    10441 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/11-09.txt
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/11-10.txt
--rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/12-01.txt
--rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/12-02.txt
--rw-r--r--   0        0        0     7772 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/12-03.txt
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/12-04.txt
--rw-r--r--   0        0        0     8098 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/12-05.txt
--rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/12-06.txt
--rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/12-07.txt
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/12-08.txt
--rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/12-09.txt
--rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/12-10.txt
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/13-01.txt
--rw-r--r--   0        0        0    11384 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/13-02.txt
--rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/13-03.txt
--rw-r--r--   0        0        0    11449 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/13-04.txt
--rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/13-05.txt
--rw-r--r--   0        0        0    10797 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/13-06.txt
--rw-r--r--   0        0        0    11081 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/13-07.txt
--rw-r--r--   0        0        0    10600 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/13-08.txt
--rw-r--r--   0        0        0    10869 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/13-09.txt
--rw-r--r--   0        0        0    10354 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/13-10.txt
--rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/14-01.txt
--rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/14-02.txt
--rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/14-03.txt
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/14-04.txt
--rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/14-05.txt
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/14-06.txt
--rw-r--r--   0        0        0     7155 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/14-07.txt
--rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/14-08.txt
--rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/14-09.txt
--rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/14-10.txt
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/15-01.txt
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/15-02.txt
--rw-r--r--   0        0        0     8932 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/15-03.txt
--rw-r--r--   0        0        0     8862 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/15-04.txt
--rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/15-05.txt
--rw-r--r--   0        0        0     8874 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/15-06.txt
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/15-07.txt
--rw-r--r--   0        0        0     8970 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/15-08.txt
--rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/15-09.txt
--rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/15-10.txt
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/16-01.txt
--rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/16-02.txt
--rw-r--r--   0        0        0     7042 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/16-03.txt
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/16-04.txt
--rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/16-05.txt
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/16-06.txt
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/16-07.txt
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/16-08.txt
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/16-09.txt
--rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/16-10.txt
--rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/17-01.txt
--rw-r--r--   0        0        0     8761 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/17-02.txt
--rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/17-03.txt
--rw-r--r--   0        0        0     8643 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/17-04.txt
--rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/17-05.txt
--rw-r--r--   0        0        0     8633 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/17-06.txt
--rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/17-07.txt
--rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/17-08.txt
--rw-r--r--   0        0        0     8442 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/17-09.txt
--rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/17-10.txt
--rw-r--r--   0        0        0     8430 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/18-01.txt
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/18-02.txt
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/18-03.txt
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/18-04.txt
--rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/18-05.txt
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/18-06.txt
--rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/18-07.txt
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/18-08.txt
--rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/18-09.txt
--rw-r--r--   0        0        0     8350 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/18-10.txt
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/19-01.txt
--rw-r--r--   0        0        0     7666 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/19-02.txt
--rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/19-03.txt
--rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/19-04.txt
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/19-05.txt
--rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/19-06.txt
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/19-07.txt
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/19-08.txt
--rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/19-09.txt
--rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/19-10.txt
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/20-01.txt
--rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/20-02.txt
--rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/20-03.txt
--rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/20-04.txt
--rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/20-05.txt
--rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/20-06.txt
--rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/20-07.txt
--rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/20-08.txt
--rw-r--r--   0        0        0     7753 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/20-09.txt
--rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/20-10.txt
--rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/21-01.txt
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/21-02.txt
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/21-03.txt
--rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/21-04.txt
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/21-05.txt
--rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/21-06.txt
--rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/21-07.txt
--rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/21-08.txt
--rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/21-09.txt
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/21-10.txt
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/22-01.txt
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/22-02.txt
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/22-03.txt
--rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/22-04.txt
--rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/22-05.txt
--rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/22-06.txt
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/22-07.txt
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/22-08.txt
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/22-09.txt
--rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/22-10.txt
--rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/23-01.txt
--rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/23-02.txt
--rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/23-03.txt
--rw-r--r--   0        0        0     9277 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/23-04.txt
--rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/23-05.txt
--rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/23-06.txt
--rw-r--r--   0        0        0     9406 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/23-07.txt
--rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/23-08.txt
--rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/23-09.txt
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/23-10.txt
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/24-01.txt
--rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/24-02.txt
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/24-03.txt
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/24-04.txt
--rw-r--r--   0        0        0     7332 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/24-05.txt
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/24-06.txt
--rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/24-07.txt
--rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/24-08.txt
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/24-09.txt
--rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/24-10.txt
--rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/25-01.txt
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/25-02.txt
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/25-03.txt
--rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/25-04.txt
--rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/25-05.txt
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/25-06.txt
--rw-r--r--   0        0        0     6287 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/25-07.txt
--rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/25-08.txt
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/25-09.txt
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/25-10.txt
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/26-01.txt
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/26-02.txt
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/26-03.txt
--rw-r--r--   0        0        0     7493 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/26-04.txt
--rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/26-05.txt
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/26-06.txt
--rw-r--r--   0        0        0     7227 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/26-07.txt
--rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/26-08.txt
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/26-09.txt
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/26-10.txt
--rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/27-01.txt
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/27-02.txt
--rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/27-03.txt
--rw-r--r--   0        0        0     6724 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/27-04.txt
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/27-05.txt
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/27-06.txt
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/27-07.txt
--rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/27-08.txt
--rw-r--r--   0        0        0     5865 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/27-09.txt
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/27-10.txt
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/28-01.txt
--rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/28-02.txt
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/28-03.txt
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/28-04.txt
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/28-05.txt
--rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/28-06.txt
--rw-r--r--   0        0        0     6046 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/28-07.txt
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/28-08.txt
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/28-09.txt
--rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM1/28-10.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/.DS_Store
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/01-01.txt
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/01-02.txt
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/01-03.txt
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/01-04.txt
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/01-05.txt
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/01-06.txt
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/01-07.txt
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/01-08.txt
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/01-09.txt
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/01-10.txt
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/02-01.txt
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/02-02.txt
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/02-03.txt
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/02-04.txt
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/02-05.txt
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/02-06.txt
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/02-07.txt
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/02-08.txt
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/02-09.txt
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/02-10.txt
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/03-01.txt
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/03-02.txt
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/03-03.txt
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/03-04.txt
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/03-05.txt
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/03-06.txt
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/03-07.txt
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/03-08.txt
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/03-09.txt
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/03-10.txt
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/04-01.txt
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/04-02.txt
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/04-03.txt
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/04-04.txt
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/04-05.txt
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/04-06.txt
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/04-07.txt
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/04-08.txt
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/04-09.txt
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/04-10.txt
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/05-01.txt
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/05-02.txt
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/05-03.txt
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/05-04.txt
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/05-05.txt
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/05-06.txt
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/05-07.txt
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/05-08.txt
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/05-09.txt
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/05-10.txt
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/06-01.txt
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/06-02.txt
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/06-03.txt
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/06-04.txt
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/06-05.txt
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/06-06.txt
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/06-07.txt
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/06-08.txt
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/06-09.txt
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/06-10.txt
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/07-01.txt
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/07-02.txt
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/07-03.txt
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/07-04.txt
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/07-05.txt
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/07-06.txt
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/07-07.txt
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/07-08.txt
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/07-09.txt
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/07-10.txt
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/08-01.txt
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/08-02.txt
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/08-03.txt
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/08-04.txt
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/08-05.txt
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/08-06.txt
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/08-07.txt
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/08-08.txt
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/08-09.txt
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/08-10.txt
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/09-01.txt
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/09-02.txt
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/09-03.txt
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/09-04.txt
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/09-05.txt
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/09-06.txt
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/09-07.txt
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/09-08.txt
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/09-09.txt
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/09-10.txt
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/10-01.txt
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/10-02.txt
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/10-03.txt
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/10-04.txt
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/10-05.txt
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/10-06.txt
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/10-07.txt
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/10-08.txt
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/10-09.txt
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/10-10.txt
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/11-01.txt
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/11-02.txt
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/11-03.txt
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/11-04.txt
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/11-05.txt
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/11-06.txt
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/11-07.txt
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/11-08.txt
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/11-09.txt
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/11-10.txt
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/12-01.txt
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/12-02.txt
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/12-03.txt
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/12-04.txt
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/12-05.txt
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/12-06.txt
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/12-07.txt
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/12-08.txt
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/12-09.txt
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/12-10.txt
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/13-01.txt
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/13-02.txt
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/13-03.txt
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/13-04.txt
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/13-05.txt
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/13-06.txt
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/13-07.txt
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/13-08.txt
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/13-09.txt
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/13-10.txt
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/14-01.txt
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/14-02.txt
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/14-03.txt
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/14-04.txt
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/14-05.txt
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/14-06.txt
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/14-07.txt
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/14-08.txt
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/14-09.txt
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/14-10.txt
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/15-01.txt
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/15-02.txt
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/15-03.txt
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/15-04.txt
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/15-05.txt
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/15-06.txt
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/15-07.txt
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/15-08.txt
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/15-09.txt
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/15-10.txt
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/16-01.txt
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/16-02.txt
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/16-03.txt
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/16-04.txt
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/16-05.txt
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/16-06.txt
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/16-07.txt
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/16-08.txt
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/16-09.txt
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/16-10.txt
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/17-01.txt
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/17-02.txt
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/17-03.txt
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/17-04.txt
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/17-05.txt
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/17-06.txt
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/17-07.txt
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/17-08.txt
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/17-09.txt
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/17-10.txt
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/18-01.txt
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/18-02.txt
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/18-03.txt
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/18-04.txt
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/18-05.txt
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/18-06.txt
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/18-07.txt
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/18-08.txt
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/18-09.txt
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/18-10.txt
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/19-01.txt
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/19-02.txt
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/19-03.txt
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/19-04.txt
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/19-05.txt
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/19-06.txt
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/19-07.txt
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/19-08.txt
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/19-09.txt
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/19-10.txt
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/20-01.txt
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/20-02.txt
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/20-03.txt
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/20-04.txt
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/20-05.txt
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/20-06.txt
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/20-07.txt
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/20-08.txt
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/20-09.txt
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/20-10.txt
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/21-01.txt
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/21-02.txt
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/21-03.txt
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/21-04.txt
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/21-05.txt
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/21-06.txt
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/21-07.txt
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/21-08.txt
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/21-09.txt
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/21-10.txt
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/22-01.txt
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/22-02.txt
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/22-03.txt
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/22-04.txt
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/22-05.txt
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/22-06.txt
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/22-07.txt
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/22-08.txt
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/22-09.txt
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/22-10.txt
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/23-01.txt
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/23-02.txt
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/23-03.txt
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/23-04.txt
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/23-05.txt
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/23-06.txt
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/23-07.txt
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/23-08.txt
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/23-09.txt
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/23-10.txt
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/24-01.txt
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/24-02.txt
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/24-03.txt
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/24-04.txt
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/24-05.txt
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/24-06.txt
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/24-07.txt
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/24-08.txt
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/24-09.txt
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/24-10.txt
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/25-01.txt
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/25-02.txt
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/25-03.txt
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/25-04.txt
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/25-05.txt
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/25-06.txt
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/25-07.txt
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/25-08.txt
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/25-09.txt
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/25-10.txt
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/26-01.txt
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/26-02.txt
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/26-03.txt
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/26-04.txt
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/26-05.txt
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/26-06.txt
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/26-07.txt
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/26-08.txt
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/26-09.txt
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/26-10.txt
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/27-01.txt
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/27-02.txt
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/27-03.txt
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/27-04.txt
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/27-05.txt
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/27-06.txt
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/27-07.txt
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/27-08.txt
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/27-09.txt
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/27-10.txt
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/28-01.txt
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/28-02.txt
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/28-03.txt
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/28-04.txt
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/28-05.txt
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/28-06.txt
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/28-07.txt
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/28-08.txt
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/28-09.txt
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/28-10.txt
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/29-01.txt
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/29-02.txt
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/29-03.txt
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/29-04.txt
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/29-05.txt
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/29-06.txt
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/29-07.txt
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/29-08.txt
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/29-09.txt
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/29-10.txt
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/30-01.txt
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/30-02.txt
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/30-03.txt
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/30-04.txt
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/30-05.txt
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/30-06.txt
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/30-07.txt
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/30-08.txt
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/30-09.txt
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/30-10.txt
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/31-01.txt
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/31-02.txt
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/31-03.txt
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/31-04.txt
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/31-05.txt
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/31-06.txt
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/31-07.txt
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/31-08.txt
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/31-09.txt
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/31-10.txt
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/32-01.txt
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/32-02.txt
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/32-03.txt
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/32-04.txt
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/32-05.txt
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/32-06.txt
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/32-07.txt
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/32-08.txt
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/32-09.txt
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/32-10.txt
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/33-01.txt
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/33-02.txt
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/33-03.txt
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/33-04.txt
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/33-05.txt
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/33-06.txt
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/33-07.txt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/33-08.txt
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/33-09.txt
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/33-10.txt
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/34-01.txt
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/34-02.txt
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/34-03.txt
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/34-04.txt
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/34-05.txt
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/34-06.txt
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/34-07.txt
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/34-08.txt
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/34-09.txt
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/34-10.txt
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/35-01.txt
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/35-02.txt
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/35-03.txt
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/35-04.txt
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/35-05.txt
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/35-06.txt
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/35-07.txt
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/35-08.txt
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/35-09.txt
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/35-10.txt
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/36-01.txt
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/36-02.txt
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/36-03.txt
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/36-04.txt
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/36-05.txt
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/36-06.txt
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/36-07.txt
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/36-08.txt
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/36-09.txt
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/36-10.txt
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/37-01.txt
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/37-02.txt
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/37-03.txt
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/37-04.txt
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/37-05.txt
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/37-06.txt
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/37-07.txt
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/37-08.txt
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/37-09.txt
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/37-10.txt
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/38-01.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/38-02.txt
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/38-03.txt
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/38-04.txt
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/38-05.txt
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/38-06.txt
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/38-07.txt
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/38-08.txt
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/38-09.txt
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/38-10.txt
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/39-01.txt
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/39-02.txt
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/39-03.txt
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/39-04.txt
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/39-05.txt
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/39-06.txt
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/39-07.txt
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/39-08.txt
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/39-09.txt
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/39-10.txt
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/40-01.txt
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/40-02.txt
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/40-03.txt
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/40-04.txt
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/40-05.txt
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/40-06.txt
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/40-07.txt
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/40-08.txt
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/40-09.txt
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/40-10.txt
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/41-01.txt
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/41-02.txt
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/41-03.txt
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/41-04.txt
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/41-05.txt
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/41-06.txt
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/41-07.txt
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/41-08.txt
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/41-09.txt
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/41-10.txt
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/43-01.txt
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/43-02.txt
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/43-03.txt
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/43-04.txt
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/43-05.txt
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/43-06.txt
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/43-07.txt
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/43-08.txt
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/43-09.txt
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/43-10.txt
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/44-01.txt
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/44-02.txt
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/44-03.txt
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/44-04.txt
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/44-05.txt
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/44-06.txt
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/44-07.txt
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/44-08.txt
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/44-09.txt
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/44-10.txt
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/45-01.txt
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/45-02.txt
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/45-03.txt
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/45-04.txt
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/45-05.txt
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/45-06.txt
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/45-07.txt
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/45-08.txt
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/45-09.txt
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/45-10.txt
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/46-01.txt
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/46-02.txt
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/46-03.txt
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/46-04.txt
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/46-05.txt
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/46-06.txt
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/46-07.txt
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/46-08.txt
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/46-09.txt
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/46-10.txt
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/47-01.txt
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/47-02.txt
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/47-03.txt
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/47-04.txt
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/47-05.txt
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/47-06.txt
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/47-07.txt
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/47-08.txt
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/47-09.txt
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/47-10.txt
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/48-01.txt
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/48-02.txt
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/48-03.txt
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/48-04.txt
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/48-05.txt
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/48-06.txt
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/48-07.txt
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/48-08.txt
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/48-09.txt
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/48-10.txt
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/49-01.txt
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/49-02.txt
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/49-03.txt
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/49-04.txt
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/49-05.txt
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/49-06.txt
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/49-07.txt
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/49-08.txt
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/49-09.txt
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/49-10.txt
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/50-01.txt
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/50-02.txt
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/50-03.txt
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/50-04.txt
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/50-05.txt
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/50-06.txt
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/50-07.txt
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/50-08.txt
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/50-09.txt
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/50-10.txt
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/51-01.txt
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/51-02.txt
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/51-03.txt
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/51-04.txt
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/51-05.txt
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/51-06.txt
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/51-07.txt
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/51-08.txt
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/51-09.txt
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/51-10.txt
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/52-01.txt
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/52-02.txt
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/52-03.txt
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/52-04.txt
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/52-05.txt
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/52-06.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/52-07.txt
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/52-08.txt
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/52-09.txt
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/52-10.txt
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/53-01.txt
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/53-02.txt
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/53-03.txt
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/53-04.txt
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/53-05.txt
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/53-06.txt
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/53-07.txt
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/53-08.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/53-09.txt
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/53-10.txt
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/54-01.txt
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/54-02.txt
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/54-03.txt
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/54-04.txt
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/54-05.txt
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/54-06.txt
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/54-07.txt
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/54-08.txt
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/54-09.txt
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/54-10.txt
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/55-01.txt
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/55-02.txt
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/55-03.txt
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/55-04.txt
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/55-05.txt
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/55-06.txt
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/55-07.txt
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/55-08.txt
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/55-09.txt
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/55-10.txt
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/56-01.txt
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/56-02.txt
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/56-03.txt
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/56-04.txt
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/56-05.txt
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/56-06.txt
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/56-07.txt
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/56-08.txt
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/56-09.txt
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/56-10.txt
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/57-01.txt
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/57-02.txt
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/57-03.txt
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/57-04.txt
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/57-05.txt
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/57-06.txt
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/57-07.txt
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/57-08.txt
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/57-09.txt
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/57-10.txt
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/58-01.txt
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/58-02.txt
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/58-03.txt
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/58-04.txt
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/58-05.txt
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/58-06.txt
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/58-07.txt
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/58-08.txt
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/58-09.txt
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/58-10.txt
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/59-01.txt
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/59-02.txt
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/59-03.txt
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/59-04.txt
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/59-05.txt
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/59-06.txt
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/59-07.txt
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/59-08.txt
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/59-09.txt
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM2/59-10.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/.DS_Store
--rw-r--r--   0        0        0    13893 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/01-01.txt
--rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/01-02.txt
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/01-03.txt
--rw-r--r--   0        0        0    13455 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/01-04.txt
--rw-r--r--   0        0        0    14133 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/01-05.txt
--rw-r--r--   0        0        0    13270 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/01-06.txt
--rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/01-07.txt
--rw-r--r--   0        0        0    15266 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/01-08.txt
--rw-r--r--   0        0        0    14566 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/01-09.txt
--rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/01-10.txt
--rw-r--r--   0        0        0    16113 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/02-01.txt
--rw-r--r--   0        0        0    15195 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/02-02.txt
--rw-r--r--   0        0        0    15103 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/02-03.txt
--rw-r--r--   0        0        0    15200 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/02-04.txt
--rw-r--r--   0        0        0    15227 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/02-05.txt
--rw-r--r--   0        0        0    14742 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/02-06.txt
--rw-r--r--   0        0        0    14482 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/02-07.txt
--rw-r--r--   0        0        0    14117 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/02-08.txt
--rw-r--r--   0        0        0    14086 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/02-09.txt
--rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/02-10.txt
--rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/03-01.txt
--rw-r--r--   0        0        0    15749 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/03-02.txt
--rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/03-03.txt
--rw-r--r--   0        0        0    15885 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/03-04.txt
--rw-r--r--   0        0        0    14187 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/03-05.txt
--rw-r--r--   0        0        0    15733 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/03-06.txt
--rw-r--r--   0        0        0    15082 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/03-07.txt
--rw-r--r--   0        0        0    15597 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/03-08.txt
--rw-r--r--   0        0        0    14720 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/03-09.txt
--rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/03-10.txt
--rw-r--r--   0        0        0    16005 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/04-01.txt
--rw-r--r--   0        0        0    16310 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/04-02.txt
--rw-r--r--   0        0        0    15306 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/04-03.txt
--rw-r--r--   0        0        0    15682 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/04-04.txt
--rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/04-05.txt
--rw-r--r--   0        0        0    15867 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/04-06.txt
--rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/04-07.txt
--rw-r--r--   0        0        0    15423 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/04-08.txt
--rw-r--r--   0        0        0    14762 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/04-09.txt
--rw-r--r--   0        0        0    15922 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/04-10.txt
--rw-r--r--   0        0        0    16891 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/05-01.txt
--rw-r--r--   0        0        0    16849 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/05-02.txt
--rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/05-03.txt
--rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/05-04.txt
--rw-r--r--   0        0        0    14097 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/05-05.txt
--rw-r--r--   0        0        0    15729 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/05-06.txt
--rw-r--r--   0        0        0    15987 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/05-07.txt
--rw-r--r--   0        0        0    15820 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/05-08.txt
--rw-r--r--   0        0        0    14857 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/05-09.txt
--rw-r--r--   0        0        0    15262 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/05-10.txt
--rw-r--r--   0        0        0    17403 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/06-01.txt
--rw-r--r--   0        0        0    17229 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/06-02.txt
--rw-r--r--   0        0        0    17591 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/06-03.txt
--rw-r--r--   0        0        0    17611 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/06-04.txt
--rw-r--r--   0        0        0    14787 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/06-05.txt
--rw-r--r--   0        0        0    17752 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/06-06.txt
--rw-r--r--   0        0        0    17700 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/06-07.txt
--rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/06-08.txt
--rw-r--r--   0        0        0    15244 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/06-09.txt
--rw-r--r--   0        0        0    17731 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/06-10.txt
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/07-01.txt
--rw-r--r--   0        0        0    19577 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/07-02.txt
--rw-r--r--   0        0        0    18971 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/07-03.txt
--rw-r--r--   0        0        0    18916 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/07-04.txt
--rw-r--r--   0        0        0    16835 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/07-05.txt
--rw-r--r--   0        0        0    19576 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/07-06.txt
--rw-r--r--   0        0        0    18859 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/07-07.txt
--rw-r--r--   0        0        0    19465 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/07-08.txt
--rw-r--r--   0        0        0    17027 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/07-09.txt
--rw-r--r--   0        0        0    19198 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/07-10.txt
--rw-r--r--   0        0        0    21655 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/08-01.txt
--rw-r--r--   0        0        0    20765 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/08-02.txt
--rw-r--r--   0        0        0    20839 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/08-03.txt
--rw-r--r--   0        0        0    19291 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/08-04.txt
--rw-r--r--   0        0        0    18508 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/08-05.txt
--rw-r--r--   0        0        0    20243 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/08-06.txt
--rw-r--r--   0        0        0    19675 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/08-07.txt
--rw-r--r--   0        0        0    20476 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/08-08.txt
--rw-r--r--   0        0        0    18453 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/08-09.txt
--rw-r--r--   0        0        0    20113 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/08-10.txt
--rw-r--r--   0        0        0    13550 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/09-01.txt
--rw-r--r--   0        0        0    14136 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/09-02.txt
--rw-r--r--   0        0        0    13167 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/09-03.txt
--rw-r--r--   0        0        0    14150 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/09-04.txt
--rw-r--r--   0        0        0    13581 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/09-05.txt
--rw-r--r--   0        0        0    13726 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/09-06.txt
--rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/09-07.txt
--rw-r--r--   0        0        0    14500 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/09-08.txt
--rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/09-09.txt
--rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/09-10.txt
--rw-r--r--   0        0        0    12470 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/10-01.txt
--rw-r--r--   0        0        0    11933 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/10-02.txt
--rw-r--r--   0        0        0    13018 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/10-03.txt
--rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/10-04.txt
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/10-05.txt
--rw-r--r--   0        0        0    12401 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/10-06.txt
--rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/10-07.txt
--rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/10-08.txt
--rw-r--r--   0        0        0    12547 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/10-09.txt
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/10-10.txt
--rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/11-01.txt
--rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/11-02.txt
--rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/11-03.txt
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/11-04.txt
--rw-r--r--   0        0        0    14145 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/11-05.txt
--rw-r--r--   0        0        0    14479 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/11-06.txt
--rw-r--r--   0        0        0    13868 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/11-07.txt
--rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/11-08.txt
--rw-r--r--   0        0        0    13379 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/11-09.txt
--rw-r--r--   0        0        0    13899 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/11-10.txt
--rw-r--r--   0        0        0    14822 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/12-01.txt
--rw-r--r--   0        0        0    14554 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/12-02.txt
--rw-r--r--   0        0        0    13942 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/12-03.txt
--rw-r--r--   0        0        0    14704 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/12-04.txt
--rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/12-05.txt
--rw-r--r--   0        0        0    15058 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/12-06.txt
--rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/12-07.txt
--rw-r--r--   0        0        0    14746 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/12-08.txt
--rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/12-09.txt
--rw-r--r--   0        0        0    14812 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/12-10.txt
--rw-r--r--   0        0        0    14129 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/13-01.txt
--rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/13-02.txt
--rw-r--r--   0        0        0    13908 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/13-03.txt
--rw-r--r--   0        0        0    14056 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/13-04.txt
--rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/13-05.txt
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/13-06.txt
--rw-r--r--   0        0        0    14460 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/13-07.txt
--rw-r--r--   0        0        0    13977 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/13-08.txt
--rw-r--r--   0        0        0    14367 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/13-09.txt
--rw-r--r--   0        0        0    13722 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/13-10.txt
--rw-r--r--   0        0        0    16072 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/14-01.txt
--rw-r--r--   0        0        0    14926 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/14-02.txt
--rw-r--r--   0        0        0    15304 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/14-03.txt
--rw-r--r--   0        0        0    15314 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/14-04.txt
--rw-r--r--   0        0        0    15726 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/14-05.txt
--rw-r--r--   0        0        0    14934 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/14-06.txt
--rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/14-07.txt
--rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/14-08.txt
--rw-r--r--   0        0        0    14606 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/14-09.txt
--rw-r--r--   0        0        0    14853 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/14-10.txt
--rw-r--r--   0        0        0    16089 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/15-01.txt
--rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/15-02.txt
--rw-r--r--   0        0        0    15083 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/15-03.txt
--rw-r--r--   0        0        0    14893 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/15-04.txt
--rw-r--r--   0        0        0    16005 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/15-05.txt
--rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/15-06.txt
--rw-r--r--   0        0        0    15746 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/15-07.txt
--rw-r--r--   0        0        0    14856 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/15-08.txt
--rw-r--r--   0        0        0    14958 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/15-09.txt
--rw-r--r--   0        0        0    14868 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/15-10.txt
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/16-01.txt
--rw-r--r--   0        0        0    17046 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/16-02.txt
--rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/16-03.txt
--rw-r--r--   0        0        0    16328 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/16-04.txt
--rw-r--r--   0        0        0    17024 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/16-05.txt
--rw-r--r--   0        0        0    16663 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/16-06.txt
--rw-r--r--   0        0        0    16545 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/16-07.txt
--rw-r--r--   0        0        0    17019 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/16-08.txt
--rw-r--r--   0        0        0    16526 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/16-09.txt
--rw-r--r--   0        0        0    15927 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/16-10.txt
--rw-r--r--   0        0        0    11749 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/17-01.txt
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/17-02.txt
--rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/17-03.txt
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/17-04.txt
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/17-05.txt
--rw-r--r--   0        0        0    11709 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/17-06.txt
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/17-07.txt
--rw-r--r--   0        0        0    11952 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/17-08.txt
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/17-09.txt
--rw-r--r--   0        0        0    12053 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/17-10.txt
--rw-r--r--   0        0        0    14592 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/18-01.txt
--rw-r--r--   0        0        0    15190 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/18-02.txt
--rw-r--r--   0        0        0    14194 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/18-03.txt
--rw-r--r--   0        0        0    14134 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/18-04.txt
--rw-r--r--   0        0        0    14959 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/18-05.txt
--rw-r--r--   0        0        0    14852 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/18-06.txt
--rw-r--r--   0        0        0    14583 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/18-07.txt
--rw-r--r--   0        0        0    14470 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/18-08.txt
--rw-r--r--   0        0        0    14357 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/18-09.txt
--rw-r--r--   0        0        0    14488 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/18-10.txt
--rw-r--r--   0        0        0    13279 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/19-01.txt
--rw-r--r--   0        0        0    13349 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/19-02.txt
--rw-r--r--   0        0        0    12956 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/19-03.txt
--rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/19-04.txt
--rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/19-05.txt
--rw-r--r--   0        0        0    13145 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/19-06.txt
--rw-r--r--   0        0        0    13465 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/19-07.txt
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/19-08.txt
--rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/19-09.txt
--rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/19-10.txt
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/20-01.txt
--rw-r--r--   0        0        0    14158 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/20-02.txt
--rw-r--r--   0        0        0    13400 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/20-03.txt
--rw-r--r--   0        0        0    13959 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/20-04.txt
--rw-r--r--   0        0        0    14215 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/20-05.txt
--rw-r--r--   0        0        0    14170 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/20-06.txt
--rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/20-07.txt
--rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/20-08.txt
--rw-r--r--   0        0        0    13772 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/20-09.txt
--rw-r--r--   0        0        0    13647 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/20-10.txt
--rw-r--r--   0        0        0    15137 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/21-01.txt
--rw-r--r--   0        0        0    14732 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/21-02.txt
--rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/21-03.txt
--rw-r--r--   0        0        0    14498 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/21-04.txt
--rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/21-05.txt
--rw-r--r--   0        0        0    15173 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/21-06.txt
--rw-r--r--   0        0        0    15155 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/21-07.txt
--rw-r--r--   0        0        0    15211 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/21-08.txt
--rw-r--r--   0        0        0    15274 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/21-09.txt
--rw-r--r--   0        0        0    15215 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/21-10.txt
--rw-r--r--   0        0        0    13228 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/22-01.txt
--rw-r--r--   0        0        0    13372 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/22-02.txt
--rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/22-03.txt
--rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/22-04.txt
--rw-r--r--   0        0        0    13190 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/22-05.txt
--rw-r--r--   0        0        0    12575 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/22-06.txt
--rw-r--r--   0        0        0    12767 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/22-07.txt
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/22-08.txt
--rw-r--r--   0        0        0    13014 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/22-09.txt
--rw-r--r--   0        0        0    12453 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/22-10.txt
--rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/23-01.txt
--rw-r--r--   0        0        0    14786 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/23-02.txt
--rw-r--r--   0        0        0    15624 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/23-03.txt
--rw-r--r--   0        0        0    15092 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/23-04.txt
--rw-r--r--   0        0        0    15274 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/23-05.txt
--rw-r--r--   0        0        0    15739 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/23-06.txt
--rw-r--r--   0        0        0    14447 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/23-07.txt
--rw-r--r--   0        0        0    14506 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/23-08.txt
--rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/23-09.txt
--rw-r--r--   0        0        0    13929 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/23-10.txt
--rw-r--r--   0        0        0    16289 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/24-01.txt
--rw-r--r--   0        0        0    16101 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/24-02.txt
--rw-r--r--   0        0        0    15257 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/24-03.txt
--rw-r--r--   0        0        0    15561 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/24-04.txt
--rw-r--r--   0        0        0    15991 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/24-05.txt
--rw-r--r--   0        0        0    15681 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/24-06.txt
--rw-r--r--   0        0        0    15713 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/24-07.txt
--rw-r--r--   0        0        0    15668 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/24-08.txt
--rw-r--r--   0        0        0    16156 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/24-09.txt
--rw-r--r--   0        0        0    15302 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/24-10.txt
--rw-r--r--   0        0        0    12206 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/25-01.txt
--rw-r--r--   0        0        0    12485 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/25-02.txt
--rw-r--r--   0        0        0    12280 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/25-03.txt
--rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/25-04.txt
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/25-05.txt
--rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/25-06.txt
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/25-07.txt
--rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/25-08.txt
--rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/25-09.txt
--rw-r--r--   0        0        0    11940 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/25-10.txt
--rw-r--r--   0        0        0    13043 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/26-01.txt
--rw-r--r--   0        0        0    12985 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/26-02.txt
--rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/26-03.txt
--rw-r--r--   0        0        0    13523 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/26-04.txt
--rw-r--r--   0        0        0    13500 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/26-05.txt
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/26-06.txt
--rw-r--r--   0        0        0    12905 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/26-07.txt
--rw-r--r--   0        0        0    13361 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/26-08.txt
--rw-r--r--   0        0        0    12843 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/26-09.txt
--rw-r--r--   0        0        0    12872 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/26-10.txt
--rw-r--r--   0        0        0    13521 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/27-01.txt
--rw-r--r--   0        0        0    13740 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/27-02.txt
--rw-r--r--   0        0        0    13580 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/27-03.txt
--rw-r--r--   0        0        0    14012 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/27-04.txt
--rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/27-05.txt
--rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/27-06.txt
--rw-r--r--   0        0        0    13933 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/27-07.txt
--rw-r--r--   0        0        0    13412 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/27-08.txt
--rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/27-09.txt
--rw-r--r--   0        0        0    13294 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/27-10.txt
--rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/28-01.txt
--rw-r--r--   0        0        0    13667 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/28-02.txt
--rw-r--r--   0        0        0    13768 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/28-03.txt
--rw-r--r--   0        0        0    13584 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/28-04.txt
--rw-r--r--   0        0        0    14038 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/28-05.txt
--rw-r--r--   0        0        0    13619 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/28-06.txt
--rw-r--r--   0        0        0    13232 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/28-07.txt
--rw-r--r--   0        0        0    13002 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/28-08.txt
--rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/28-09.txt
--rw-r--r--   0        0        0    13835 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/28-10.txt
--rw-r--r--   0        0        0    13902 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/29-01.txt
--rw-r--r--   0        0        0    14555 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/29-02.txt
--rw-r--r--   0        0        0    13917 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/29-03.txt
--rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/29-04.txt
--rw-r--r--   0        0        0    14069 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/29-05.txt
--rw-r--r--   0        0        0    14093 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/29-06.txt
--rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/29-07.txt
--rw-r--r--   0        0        0    14397 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/29-08.txt
--rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/29-09.txt
--rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/29-10.txt
--rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/30-01.txt
--rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/30-02.txt
--rw-r--r--   0        0        0    14606 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/30-03.txt
--rw-r--r--   0        0        0    15683 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/30-04.txt
--rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/30-05.txt
--rw-r--r--   0        0        0    14758 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/30-06.txt
--rw-r--r--   0        0        0    14905 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/30-07.txt
--rw-r--r--   0        0        0    15390 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/30-08.txt
--rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/30-09.txt
--rw-r--r--   0        0        0    15364 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/30-10.txt
--rw-r--r--   0        0        0    15015 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/31-01.txt
--rw-r--r--   0        0        0    14118 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/31-02.txt
--rw-r--r--   0        0        0    14075 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/31-03.txt
--rw-r--r--   0        0        0    14044 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/31-04.txt
--rw-r--r--   0        0        0    15092 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/31-05.txt
--rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/31-06.txt
--rw-r--r--   0        0        0    14001 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/31-07.txt
--rw-r--r--   0        0        0    13472 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/31-08.txt
--rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/31-09.txt
--rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/31-10.txt
--rw-r--r--   0        0        0    12935 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/32-01.txt
--rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/32-02.txt
--rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/32-03.txt
--rw-r--r--   0        0        0    13063 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/32-04.txt
--rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/32-05.txt
--rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/32-06.txt
--rw-r--r--   0        0        0    12966 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/32-07.txt
--rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/32-08.txt
--rw-r--r--   0        0        0    12332 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/32-09.txt
--rw-r--r--   0        0        0    12070 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/32-10.txt
--rw-r--r--   0        0        0    12649 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/33-01.txt
--rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/33-02.txt
--rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/33-03.txt
--rw-r--r--   0        0        0    12399 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/33-04.txt
--rw-r--r--   0        0        0    12834 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/33-05.txt
--rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/33-06.txt
--rw-r--r--   0        0        0    13207 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/33-07.txt
--rw-r--r--   0        0        0    12644 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/33-08.txt
--rw-r--r--   0        0        0    12931 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/33-09.txt
--rw-r--r--   0        0        0    13148 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/33-10.txt
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/34-01.txt
--rw-r--r--   0        0        0    13794 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/34-02.txt
--rw-r--r--   0        0        0    13861 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/34-03.txt
--rw-r--r--   0        0        0    13897 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/34-04.txt
--rw-r--r--   0        0        0    13440 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/34-05.txt
--rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/34-06.txt
--rw-r--r--   0        0        0    14606 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/34-07.txt
--rw-r--r--   0        0        0    14283 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/34-08.txt
--rw-r--r--   0        0        0    13697 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/34-09.txt
--rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/34-10.txt
--rw-r--r--   0        0        0    14092 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/35-01.txt
--rw-r--r--   0        0        0    13845 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/35-02.txt
--rw-r--r--   0        0        0    13258 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/35-03.txt
--rw-r--r--   0        0        0    13244 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/35-04.txt
--rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/35-05.txt
--rw-r--r--   0        0        0    13395 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/35-06.txt
--rw-r--r--   0        0        0    14196 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/35-07.txt
--rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/35-08.txt
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/35-09.txt
--rw-r--r--   0        0        0    13971 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/35-10.txt
--rw-r--r--   0        0        0    14564 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/36-01.txt
--rw-r--r--   0        0        0    15125 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/36-02.txt
--rw-r--r--   0        0        0    14335 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/36-03.txt
--rw-r--r--   0        0        0    14712 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/36-04.txt
--rw-r--r--   0        0        0    14579 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/36-05.txt
--rw-r--r--   0        0        0    14061 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/36-06.txt
--rw-r--r--   0        0        0    14404 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/36-07.txt
--rw-r--r--   0        0        0    15034 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/36-08.txt
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/36-09.txt
--rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/36-10.txt
--rw-r--r--   0        0        0    15097 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/37-01.txt
--rw-r--r--   0        0        0    15988 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/37-02.txt
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/37-03.txt
--rw-r--r--   0        0        0    14612 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/37-04.txt
--rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/37-05.txt
--rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/37-06.txt
--rw-r--r--   0        0        0    13572 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/37-07.txt
--rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/37-08.txt
--rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/37-09.txt
--rw-r--r--   0        0        0    13886 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/37-10.txt
--rw-r--r--   0        0        0    16230 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/38-01.txt
--rw-r--r--   0        0        0    16550 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/38-02.txt
--rw-r--r--   0        0        0    15624 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/38-03.txt
--rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/38-04.txt
--rw-r--r--   0        0        0    15379 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/38-05.txt
--rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/38-06.txt
--rw-r--r--   0        0        0    16090 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/38-07.txt
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/38-08.txt
--rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/38-09.txt
--rw-r--r--   0        0        0    15925 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/38-10.txt
--rw-r--r--   0        0        0    18035 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/39-01.txt
--rw-r--r--   0        0        0    17900 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/39-02.txt
--rw-r--r--   0        0        0    17659 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/39-03.txt
--rw-r--r--   0        0        0    18452 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/39-04.txt
--rw-r--r--   0        0        0    18078 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/39-05.txt
--rw-r--r--   0        0        0    18039 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/39-06.txt
--rw-r--r--   0        0        0    17657 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/39-07.txt
--rw-r--r--   0        0        0    18038 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/39-08.txt
--rw-r--r--   0        0        0    18349 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/39-09.txt
--rw-r--r--   0        0        0    18471 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/39-10.txt
--rw-r--r--   0        0        0    11911 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/40-01.txt
--rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/40-02.txt
--rw-r--r--   0        0        0    11995 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/40-03.txt
--rw-r--r--   0        0        0    11426 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/40-04.txt
--rw-r--r--   0        0        0    11784 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/40-05.txt
--rw-r--r--   0        0        0    11487 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/40-06.txt
--rw-r--r--   0        0        0    12272 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/40-07.txt
--rw-r--r--   0        0        0    11666 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/40-08.txt
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/40-09.txt
--rw-r--r--   0        0        0    12995 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/40-10.txt
--rw-r--r--   0        0        0    13017 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/41-01.txt
--rw-r--r--   0        0        0    12991 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/41-02.txt
--rw-r--r--   0        0        0    13071 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/41-03.txt
--rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/41-04.txt
--rw-r--r--   0        0        0    13279 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/41-05.txt
--rw-r--r--   0        0        0    13247 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/41-06.txt
--rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/41-07.txt
--rw-r--r--   0        0        0    13537 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/41-08.txt
--rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/41-09.txt
--rw-r--r--   0        0        0    13115 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/41-10.txt
--rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/42-01.txt
--rw-r--r--   0        0        0    13675 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/42-02.txt
--rw-r--r--   0        0        0    12266 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/42-03.txt
--rw-r--r--   0        0        0    13256 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/42-04.txt
--rw-r--r--   0        0        0    12671 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/42-05.txt
--rw-r--r--   0        0        0    12404 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/42-06.txt
--rw-r--r--   0        0        0    11629 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/42-07.txt
--rw-r--r--   0        0        0    13020 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/42-08.txt
--rw-r--r--   0        0        0    12374 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/42-09.txt
--rw-r--r--   0        0        0    12306 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/42-10.txt
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/43-01.txt
--rw-r--r--   0        0        0    14654 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/43-02.txt
--rw-r--r--   0        0        0    13717 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/43-03.txt
--rw-r--r--   0        0        0    14087 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/43-04.txt
--rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/43-05.txt
--rw-r--r--   0        0        0    14249 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/43-06.txt
--rw-r--r--   0        0        0    14150 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/43-07.txt
--rw-r--r--   0        0        0    14105 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/43-08.txt
--rw-r--r--   0        0        0    14009 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/43-09.txt
--rw-r--r--   0        0        0    13660 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/43-10.txt
--rw-r--r--   0        0        0    15906 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/44-01.txt
--rw-r--r--   0        0        0    14602 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/44-02.txt
--rw-r--r--   0        0        0    14054 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/44-03.txt
--rw-r--r--   0        0        0    14402 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/44-04.txt
--rw-r--r--   0        0        0    15594 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/44-05.txt
--rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/44-06.txt
--rw-r--r--   0        0        0    14531 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/44-07.txt
--rw-r--r--   0        0        0    14465 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/44-08.txt
--rw-r--r--   0        0        0    13713 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/44-09.txt
--rw-r--r--   0        0        0    13655 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/44-10.txt
--rw-r--r--   0        0        0    16288 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/45-01.txt
--rw-r--r--   0        0        0    15597 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/45-02.txt
--rw-r--r--   0        0        0    16056 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/45-03.txt
--rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/45-04.txt
--rw-r--r--   0        0        0    16118 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/45-05.txt
--rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/45-06.txt
--rw-r--r--   0        0        0    16468 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/45-07.txt
--rw-r--r--   0        0        0    16634 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/45-08.txt
--rw-r--r--   0        0        0    16585 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/45-09.txt
--rw-r--r--   0        0        0    16356 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/45-10.txt
--rw-r--r--   0        0        0    18107 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/46-01.txt
--rw-r--r--   0        0        0    17137 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/46-02.txt
--rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/46-03.txt
--rw-r--r--   0        0        0    17983 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/46-04.txt
--rw-r--r--   0        0        0    17548 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/46-05.txt
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/46-06.txt
--rw-r--r--   0        0        0    17921 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/46-07.txt
--rw-r--r--   0        0        0    18921 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/46-08.txt
--rw-r--r--   0        0        0    17863 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/46-09.txt
--rw-r--r--   0        0        0    17898 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/46-10.txt
--rw-r--r--   0        0        0    20152 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/47-01.txt
--rw-r--r--   0        0        0    19126 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/47-02.txt
--rw-r--r--   0        0        0    19687 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/47-03.txt
--rw-r--r--   0        0        0    20597 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/47-04.txt
--rw-r--r--   0        0        0    20210 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/47-05.txt
--rw-r--r--   0        0        0    21091 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/47-06.txt
--rw-r--r--   0        0        0    20711 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/47-07.txt
--rw-r--r--   0        0        0    20630 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/47-08.txt
--rw-r--r--   0        0        0    20284 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/47-09.txt
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/47-10.txt
--rw-r--r--   0        0        0    21494 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/48-01.txt
--rw-r--r--   0        0        0    22155 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/48-02.txt
--rw-r--r--   0        0        0    21640 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/48-03.txt
--rw-r--r--   0        0        0    19896 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/48-04.txt
--rw-r--r--   0        0        0    19907 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/48-05.txt
--rw-r--r--   0        0        0    19583 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/48-06.txt
--rw-r--r--   0        0        0    19902 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/48-07.txt
--rw-r--r--   0        0        0    19913 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/48-08.txt
--rw-r--r--   0        0        0    18852 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/48-09.txt
--rw-r--r--   0        0        0    21258 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/48-10.txt
--rw-r--r--   0        0        0    15006 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/49-01.txt
--rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/49-02.txt
--rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/49-03.txt
--rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/49-04.txt
--rw-r--r--   0        0        0    14586 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/49-05.txt
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/49-06.txt
--rw-r--r--   0        0        0    14875 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/49-07.txt
--rw-r--r--   0        0        0    12851 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/49-08.txt
--rw-r--r--   0        0        0    13158 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/49-09.txt
--rw-r--r--   0        0        0    14629 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/CM3/49-10.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/.DS_Store
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/01-01.txt
--rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/01-02.txt
--rw-r--r--   0        0        0     9104 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/01-03.txt
--rw-r--r--   0        0        0     7025 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/01-04.txt
--rw-r--r--   0        0        0     7317 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/01-05.txt
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/01-06.txt
--rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/01-07.txt
--rw-r--r--   0        0        0     9367 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/01-08.txt
--rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/01-09.txt
--rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/01-10.txt
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/02-01.txt
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/02-02.txt
--rw-r--r--   0        0        0     7682 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/02-03.txt
--rw-r--r--   0        0        0     7741 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/02-04.txt
--rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/02-05.txt
--rw-r--r--   0        0        0     7611 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/02-06.txt
--rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/02-07.txt
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/02-08.txt
--rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/02-09.txt
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/02-10.txt
--rw-r--r--   0        0        0     7689 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/03-01.txt
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/03-02.txt
--rw-r--r--   0        0        0     7493 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/03-03.txt
--rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/03-04.txt
--rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/03-05.txt
--rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/03-06.txt
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/03-07.txt
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/03-08.txt
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/03-09.txt
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/03-10.txt
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/04-01.txt
--rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/04-02.txt
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/04-03.txt
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/04-04.txt
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/04-05.txt
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/04-06.txt
--rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/04-07.txt
--rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/04-08.txt
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/04-09.txt
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/04-10.txt
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/05-01.txt
--rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/05-02.txt
--rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/05-03.txt
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/05-04.txt
--rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/05-05.txt
--rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/05-06.txt
--rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/05-07.txt
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/05-08.txt
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/05-09.txt
--rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/05-10.txt
--rw-r--r--   0        0        0     7528 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/06-01.txt
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/06-02.txt
--rw-r--r--   0        0        0     8044 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/06-03.txt
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/06-04.txt
--rw-r--r--   0        0        0     7374 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/06-05.txt
--rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/06-06.txt
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/06-07.txt
--rw-r--r--   0        0        0     6937 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/06-08.txt
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/06-09.txt
--rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/06-10.txt
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/07-01.txt
--rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/07-02.txt
--rw-r--r--   0        0        0     8221 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/07-03.txt
--rw-r--r--   0        0        0     7689 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/07-04.txt
--rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/07-05.txt
--rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/07-06.txt
--rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/07-07.txt
--rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/07-08.txt
--rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/07-09.txt
--rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/07-10.txt
--rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/08-01.txt
--rw-r--r--   0        0        0     9866 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/08-02.txt
--rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/08-03.txt
--rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/08-04.txt
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/08-05.txt
--rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/08-06.txt
--rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/08-07.txt
--rw-r--r--   0        0        0     9071 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/08-08.txt
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/08-09.txt
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/08-10.txt
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/09-01.txt
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/09-02.txt
--rw-r--r--   0        0        0     5709 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/09-03.txt
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/09-04.txt
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/09-05.txt
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/09-06.txt
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/09-07.txt
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/09-08.txt
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/09-09.txt
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/09-10.txt
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/10-01.txt
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/10-02.txt
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/10-03.txt
--rw-r--r--   0        0        0     7479 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/10-04.txt
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/10-05.txt
--rw-r--r--   0        0        0     7977 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/10-06.txt
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/10-07.txt
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/10-08.txt
--rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/10-09.txt
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/10-10.txt
--rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/11-01.txt
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/11-02.txt
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/11-03.txt
--rw-r--r--   0        0        0     7641 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/11-04.txt
--rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/11-05.txt
--rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/11-06.txt
--rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/11-07.txt
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/11-08.txt
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/11-09.txt
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/11-10.txt
--rw-r--r--   0        0        0    11437 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/12-01.txt
--rw-r--r--   0        0        0    10838 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/12-02.txt
--rw-r--r--   0        0        0    11194 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/12-03.txt
--rw-r--r--   0        0        0    10366 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/12-04.txt
--rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/12-05.txt
--rw-r--r--   0        0        0    10632 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/12-06.txt
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/12-07.txt
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/12-08.txt
--rw-r--r--   0        0        0    11114 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/12-09.txt
--rw-r--r--   0        0        0    10803 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/12-10.txt
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/13-01.txt
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/13-02.txt
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/13-03.txt
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/13-04.txt
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/13-05.txt
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/13-06.txt
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/13-07.txt
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/13-08.txt
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/13-09.txt
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/13-10.txt
--rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/14-01.txt
--rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/14-02.txt
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/14-03.txt
--rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/14-04.txt
--rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/14-05.txt
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/14-06.txt
--rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/14-07.txt
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/14-08.txt
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/14-09.txt
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/14-10.txt
--rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/15-01.txt
--rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/15-02.txt
--rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/15-03.txt
--rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/15-04.txt
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/15-05.txt
--rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/15-06.txt
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/15-07.txt
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/15-08.txt
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/15-09.txt
--rw-r--r--   0        0        0     7689 2020-02-02 00:00:00.000000 hdcms-0.1.19/examples/data/Isomers/15-10.txt
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hdcms-0.1.19/out/hdcms/__init__.pyi
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 hdcms-0.1.19/out/hdcms/gen.pyi
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 hdcms-0.1.19/out/hdcms/stats.pyi
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hdcms-0.1.19/out/hdcms/verify.pyi
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 hdcms-0.1.19/out/hdcms/visualize.pyi
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 hdcms-0.1.19/src/hdcms/__init__.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 hdcms-0.1.19/src/hdcms/gen.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 hdcms-0.1.19/src/hdcms/stats.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 hdcms-0.1.19/src/hdcms/verify.py
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 hdcms-0.1.19/src/hdcms/visualize.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hdcms-0.1.19/.gitignore
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 hdcms-0.1.19/LICENSE.txt
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 hdcms-0.1.19/README.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 hdcms-0.1.19/pyproject.toml
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 hdcms-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hdcms-0.1.9/out/hdcms_helper/__init__.pyi
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hdcms-0.1.9/out/hdcms_helper/clean.pyi
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 hdcms-0.1.9/out/hdcms_helper/gen.pyi
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 hdcms-0.1.9/out/hdcms_helper/stats.pyi
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 hdcms-0.1.9/out/hdcms_helper/visualize.pyi
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hdcms-0.1.9/src/hdcms_helper/__init__.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 hdcms-0.1.9/src/hdcms_helper/clean.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 hdcms-0.1.9/src/hdcms_helper/gen.py
+-rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 hdcms-0.1.9/src/hdcms_helper/stats.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 hdcms-0.1.9/src/hdcms_helper/visualize.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 hdcms-0.1.9/test/.DS_Store
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hdcms-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 hdcms-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 hdcms-0.1.9/README.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 hdcms-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 hdcms-0.1.9/PKG-INFO
```

### Comparing `hdcms-0.1.19/.DS_Store` & `hdcms-0.1.9/test/.DS_Store`

 * *Files identical despite different names*

### Comparing `hdcms-0.1.19/out/hdcms/stats.pyi` & `hdcms-0.1.9/out/hdcms_helper/stats.pyi`

 * *Files identical despite different names*

### Comparing `hdcms-0.1.19/src/hdcms/gen.py` & `hdcms-0.1.9/src/hdcms_helper/gen.py`

 * *Files identical despite different names*

### Comparing `hdcms-0.1.19/src/hdcms/stats.py` & `hdcms-0.1.9/src/hdcms_helper/stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import hdcms_bindings
+import hdcms
 import re
 import os
 import sys
 import numpy as np
 
 def file_ok(fname):
     """ensure that fname is a file"""
     if not (os.path.isfile(fname) and os.access(fname, os.R_OK)):
         raise RuntimeError(f"File {fname} doesn't exist or isn't readable")
 
 def filenames2stats1d(filenames):
     """take filenames and convert them into a 1d summary statistic"""
     for f in filenames.split(","):
         file_ok(f)
-    return hdcms_bindings.filenames_to_stats_1d(filenames)
+    return hdcms.filenames_to_stats_1d(filenames)
 
 def filenames2stats2d(filenames):
     """take filenames and convert them into a 2d summary statistic"""
     for f in filenames.split(","):
         if not (os.path.isfile(f) and os.access(f, os.R_OK)):
             raise RuntimeError(f"File {f} doesn't exist or isn't readable")
-    return hdcms_bindings.filenames_to_stats_2d(filenames)
+    return hdcms.filenames_to_stats_2d(filenames)
 
 def regex2filenames(regex, dir="."):
     """takes regex, finds all files that match and convert them into list of filenames"""
     files = [f for f in os.listdir(dir) if os.path.isfile(os.path.join(dir, f))]
 
     r = re.compile(regex)
     matches = []
     for f in files:
         match = r.match(f)
         if match:
-            matches.append(f)
+            matches.append(match.group())
 
     if len(matches) == 0:
         raise RuntimeError(f"No matches for {regex} in directory {dir}")
 
     full_paths = list(map(lambda f: os.path.join(dir, f), matches))
     return ','.join(full_paths)
 
@@ -116,16 +116,16 @@
     # verify they all have the same length of second dimension
     for arr in args:
         if arr.shape[1] != len_of_dim_2:
             raise RuntimeError(f"Mismatch dimension: recieved {arr.shape} and {args[0].shape}, they must be the same and either (_, 2) or (_, 4)")
 
     if len(args) == 2:
         if is_using_2d:
-            return hdcms_bindings.compare_compound_2d(args[0], args[1])
+            return hdcms.compare_compound_2d(args[0], args[1])
         else:
-            return hdcms_bindings.compare_compound_1d(args[0], args[1])
+            return hdcms.compare_compound_1d(args[0], args[1])
     else:
         if is_using_2d:
-            return hdcms_bindings.compare_all_2d(args)
+            return hdcms.compare_all_2d(args)
         else:
-            return hdcms_bindings.compare_all_1d(args)
+            return hdcms.compare_all_1d(args)
```

### Comparing `hdcms-0.1.19/.gitignore` & `hdcms-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hdcms-0.1.19/LICENSE.txt` & `hdcms-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdcms-0.1.19/pyproject.toml` & `hdcms-0.1.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hdcms"
-version = "0.1.19"
+version = "0.1.9"
 description = "This package creates useful helper functions for python API"
 authors = [
     {name="Jason Eveleth", email="hdcms-helper@jasoneveleth.com"},
     {name="Arun Moorthy"},
 ]
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["hdcms-bindings", "opencv-python", "numpy", "matplotlib", "scipy"]
+dependencies = ["hdcms", "opencv-python", "numpy", "matplotlib", "scipy"]
 license = { file="LICENSE.txt" }
 
 [project.urls]
-"Homepage" = "https://github.com/jasoneveleth/hdcms-python"
-"Bug Tracker" = "https://github.com/jasoneveleth/hdcms-python/issues"
+"Homepage" = "https://github.com/jasoneveleth/pyhdcms-helper"
+"Bug Tracker" = "https://github.com/jasoneveleth/pyhdcms-helper/issues"
```

### Comparing `hdcms-0.1.19/PKG-INFO` & `hdcms-0.1.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hdcms
-Version: 0.1.19
+Version: 0.1.9
 Summary: This package creates useful helper functions for python API
-Project-URL: Homepage, https://github.com/jasoneveleth/hdcms-python
-Project-URL: Bug Tracker, https://github.com/jasoneveleth/hdcms-python/issues
+Project-URL: Homepage, https://github.com/jasoneveleth/pyhdcms-helper
+Project-URL: Bug Tracker, https://github.com/jasoneveleth/pyhdcms-helper/issues
 Author: Arun Moorthy
 Author-email: Jason Eveleth <hdcms-helper@jasoneveleth.com>
 License: NIST-developed software is provided by NIST as a public service. You may use,
         copy, and distribute copies of the software in any medium, provided that you
         keep intact this entire notice. You may improve, modify, and create derivative
         works of the software or any portion of the software, and you may copy and
         distribute such modifications or works. Modified works should carry a notice
@@ -31,57 +31,63 @@
         with applicable laws, damage to or loss of data, programs or equipment, and the
         unavailability or interruption of operation. This software is not intended to
         be used in any situation where a failure could cause risk of injury or damage
         to property. The software developed by NIST employees is not subject to
         copyright protection within the United States.
 License-File: LICENSE.txt
 Requires-Python: >=3.7
-Requires-Dist: hdcms-bindings
+Requires-Dist: hdcms
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
-# hdcms
+# hdcms-helper
 
 This library is available on pypi [here](https://pypi.org/project/hdcms/). Install using `pip install hdcms`.
 
-A very simple example:
+How to use
 
 ```python
 import hdcms as hdc
 
 hdc.generate_examples(visualize=True)
 gaussian_sum_stat = hdc.regex2stats1d(r"gaus_\d+.txt")
 laplacian_sum_stat = hdc.regex2stats1d(r"laplace_\d+\.txt")
 
+# data in another directory for example:
+# regex2stats2d(r"CM1_11_\d+.txt", dir="~/src/hdcms/data/")
+
 print(hdc.compare(gaussian_sum_stat, laplacian_sum_stat))
 hdc.write_image(gaussian_sum_stat, "tmp.png")
 ```
 
 This library is built on top of the [`hdcms-bindings` package](https://pypi.org/project/hdcms-bindings/), which exposes python bindings to a C library. That bindings package contains only a few functions and lacks a nice user experience. But, if you are only interested in that, check it out.
 
-For more documentation: see [`examples/` directory](https://github.com/jasoneveleth/hdcms-python/tree/main/examples).
+# Summary of provided functions
+
+`regex2stats1d`, `regex2stats2d` - takes regex and converts to summary statistic
+`array2stats1d`, `array2stats2d` - takes a varargs list of numpy arrays and converts them into 1d summary statistic
+`file2stats1d`, `file2stats2d` - takes filename and converts it to a summary stat. it is expected that the file contents are a list of filenames on separate lines
+`filenames2stats1d`, `filenames2stats2d` - takes list of filenames and converts it to a summary stat
+`compare` - compares two summary statistics
+`write_image` - visualizes a summary statistic
+`clean` - takes list of filenames and shows you what changes need to be made
+`generate_examples` - generate synthetic data as an example
 
 ## Dependencies
 
-`numpy` is a necessary dependency for every function. 
+Numpy is a necessary dependency for every function. 
+Matplotlib and scipy are needed for \verb|generate_example()|, which will generate a raondom synthetic data set. 
+opencv is required for \verb|write_image()|, which will visualize summary statistics. 
+You can see a complete list of functions (and where they are located) by running the following code.
+Look at the output of \verb|help(hdc)| to get the right filename.
+
+## TODO
 
-`matplotlib` and scipy are needed for `generate_example()`, which will generate a random synthetic data set. 
+filter function for 2d spectra to filter out peaks with large x variation
 
 ## Change Log
 
-```
-0.1.19 Return image from write_image
-0.1.18 Add labels to visualization configuration options
-0.1.17 Use matplotlib axes rather than my own
-0.1.16 Bug fixes (text for x axis, names for regex2filenames)
-0.1.15 Return image from write_image, rather than writing to file
-0.1.14 Add new params to write_image
-0.1.13 Add new params to write_image
-0.1.12 Add params to write_image
-0.1.11 Fix problems introduced by rename
-0.1.10 Really rename (broken)
-0.1.9 Rename, performance for visulize in 1D case (broken)
+0.1.9 Rename, performance for visulize in 1D case
 0.1.8 Add documentation
-```
```

