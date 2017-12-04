add_library(ckt acan.c cktdltm.c cktmask.c cktpname.c daskq.c noisean.c
acaskq.c    cktdltn.c   cktmcrt.c   cktpzld.c       dcoaskq.c   nsetparm.c
acsetp.c    cktdojob.c  cktmkcur.c  cktpzset.c      dcop.c      pzan.c
cktaccpt.c  cktdump.c   cktmknod.c  cktpzstr.c      dcosetp.c   pzaskq.c
cktacct.c   cktfbran.c  cktmkvol.c  cktsens.c       dctaskq.c   pzsetp.c
cktacdum.c  cktfdev.c   cktmpar.c   cktsetap.c      dctran.c    
cktask.c    cktfnda.c   cktnames.c  cktsetbk.c      dctrcurv.c  sensaskq.c
cktaskaq.c  cktfndm.c   cktnewan.c  cktsetnp.c      dctsetp.c   senssetp.c
cktasknq.c  cktfnode.c  cktneweq.c  cktsetup.c      distoan.c   tfanal.c
cktbindn.c  cktftask.c  cktnewn.c   cktsgen.c       dkerproc.c  tfaskq.c
cktbkdum.c  cktgrnd.c   cktnodn.c   cktsopt.c       dloadfns.c  tfsetp.c
cktclrbk.c  ckti2nod.c  cktnoise.c  ckttemp.c       dsetparm.c  tranaskq.c
cktcrte.c   cktic.c     cktntask.c  cktterr.c       traninit.c
cktdelt.c   cktinit.c   cktnum2n.c  ckttroub.c      transetp.c
cktdest.c   cktlnkeq.c  cktop.c     ckttrunc.c      naskq.c
cktdisto.c  cktload.c   cktparam.c  ckttyplk.c      nevalsrc.c
cktdlti.c   cktmapn.c   cktpmnam.c  ninteg.c)
include_directories(${PROJECT_SOURCE_DIR}/src/include ${PROJECT_SOURCE_DIR}/src/lib/dev)
target_link_libraries(ckt fte)
