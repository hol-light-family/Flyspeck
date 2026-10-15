# Provenance of ../ineqs.txt.
#
# ineqs/ineqs_all.txt holds all 23242 cases of the nonlinear inequalities, the
# five sharp ones included.  native_verifier settles the other 23237 by interval
# arithmetic and reads them from ../ineqs.txt, which "filter-sharp" derives by
# dropping the five:
#
#   make filter-sharp
#
# ../ineqs.txt is checked in, so this is here to say where it comes from rather
# than because anything builds it.

filter-sharp:
	sed -e '/13158,(prep-TSKAJXY-RIBCYXU sharp,0)/{d}' \
	    -e '/13077,(prep-TSKAJXY-IYOUOBF sharp v2,0)/{d}' \
	    -e '/11966,(prep-OMKYNLT 3336871894,0)/{d}' \
	    -e '/11959,(prep-GRKIBMP B V2,0)/{d}' \
	    -e '/13075,(prep-QZECFIC wt0 corner,0)/{d}' \
	    ineqs/ineqs_all.txt > ../ineqs.txt

.PHONY: filter-sharp
