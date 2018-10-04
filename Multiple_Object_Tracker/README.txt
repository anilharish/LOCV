-----------------------------Directions to compile and edit the type of tracker -------------------

1. To compile: g++ -std=c++11 multiple_object_tracker.cpp -o multiple_object_tracker `pkg-config --lis --cflags opencv`

2. To change the type of tracker: Edit the tracker name in quotes in line 61 from the reference available in lne 14. Available trackers are
   (a) BOOSTING
   (b) MIL
   (c) KCF
   (d) TLD
   (e) MEDIANFLOW
   (f) GOTURN
   (g) MOOSE
   (h) CSRT

3. To change the location or path of the source file edit the location/path inside the quotes in line 64 of the program. ACPSO is already available in the videos folder in GITHUB.
