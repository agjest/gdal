
include ../../GDALmake.opt

OBJ	=	hdf4dataset.o hdf4imagedataset.o

SUBLIBS 	= lib-hdfeos

CPPFLAGS	:=	-I../pds -Ihdf-eos $(GDAL_INCLUDE) $(HDF4_INCLUDE) $(CPPFLAGS)

default:	$(OBJ:.o=.$(OBJ_EXT)) $(SUBLIBS)

clean:
	rm -f *.o $(O_OBJ)
	(cd hdf-eos; $(MAKE) clean)

lib-hdfeos:
	(cd hdf-eos; $(MAKE) install-obj)

install-obj:	$(SUBLIBS) $(O_OBJ:.o=.$(OBJ_EXT))
