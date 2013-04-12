

include ../../../GDALmake.opt

OBJ	=	ogrsosidriver.o ogrsosidatasource.o ogrsosilayer.o ogrsosidatatypes.o 

CPPFLAGS	:=-DLINUX -DUNIX -I.. -I../.. $(GDAL_INCLUDE) $(SOSI_INC_DIR) $(CPPFLAGS)

default:	$(O_OBJ:.o=.$(OBJ_EXT))

clean:
	rm -f *.o $(O_OBJ)

$(O_OBJ):	ogr_sosi.h

