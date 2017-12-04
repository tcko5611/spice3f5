add_library(fte agraf.c     compose.c   evaluate.c  misccoms.c  points.c    subckt.c
arg.c       cpitf.c     fourier.c   miscvars.c  postcoms.c  types.c
aspice.c    debugcom.c  gens.c      newcoms.c   postsc.c    vectors.c
breakp.c    define.c    graf.c      nutctab.c   rawfile.c   where.c
breakp2.c   device.c    graphdb.c   nutinp.c    resource.c  x10.c
circuits.c  diff.c      grid.c      nutmegif.c  runcoms.c   x11.c
clip.c      dimens.c    inp.c       options.c   runcoms2.c  xgraph.c
cmath1.c    display.c   inpcom.c    outitf.c    shyu.c
cmath2.c    doplot.c    interp.c    parse.c     signal.c
cmath3.c    dotcards.c  linear.c    plot5.c     spcmdtab.c
cmath4.c    error.c     mfb.c       plotcurv.c  spiceif.c)

target_link_libraries(fte inp)
