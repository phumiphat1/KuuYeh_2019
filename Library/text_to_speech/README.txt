﻿version : 1.0
Last Edit : Yoolaibeef
Note : ทำงานได้เรียบร้อยแล้ว
Status : DONE
<< ใช้ให้มันเว้นคำ
__ ใช้ให้มันกระแทกเสียง เน้นเสียง
===================
SIMPLE CODE
--------------
import machine
import S1V30120
from pyb import SPI

SPI_2 = SPI(2, SPI.MASTER,\ baudrate=750000, polarity=1, phase=1,\ bits=8, firstbit=SPI.MSB)
TTS = S1V30120.S1V30120(SPI_2)
TTS.enableS1V()

# TEST FUNCTION HERE!
TTS.S1V30120_speech("Welcome to Fento!",0)
--------------
