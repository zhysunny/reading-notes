DIF1 := EMA(REF(C,1),SHORT) - EMA(REF(C,1),LONG);
DEA1  := EMA(DIF1,M);
DIF := EMA(C,SHORT) - EMA(C,LONG);
DEA  := EMA(DIF,M);
DIF <= DEA && DIF > DIF1 && C < 50;