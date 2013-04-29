

include ../../../GDALmake.opt

<<<<<<< HEAD
OBJ	=	ogrsosidriver.o ogrsosidatasource.o ogrsosilayer.o ogrsosidatatypes.o 
=======
OBJ	=	ogrsosidriver.o ogrsosidatasource.o ogrsosilayer.o
# ogrsosidatatypes.o 
>>>>>>> e48072bbb3d0b7e8d1e6f179d47923836558f253

CPPFLAGS	:=-DLINUX -DUNIX -I.. -I../.. $(GDAL_INCLUDE) $(SOSI_INC) $(CPPFLAGS)

default:	$(O_OBJ:.o=.$(OBJ_EXT))

clean:
	rm -f *.o $(O_OBJ)

$(O_OBJ):	ogr_sosi.h

