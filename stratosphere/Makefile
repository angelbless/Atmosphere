KIPS := loader pm sm boot fs_mitm creport

#TODO: boot2 ?

SUBFOLDERS := libstratosphere $(KIPS)

TOPTARGETS := all clean

$(TOPTARGETS): $(SUBFOLDERS)

$(SUBFOLDERS):
	$(MAKE) -C $@ $(MAKECMDGOALS)

$(KIPS): libstratosphere

.PHONY: $(TOPTARGETS) $(SUBFOLDERS)
