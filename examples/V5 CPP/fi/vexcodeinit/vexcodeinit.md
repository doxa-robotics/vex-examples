category: control  
signature: vexcodeInit();  
description: Initializes devices added using the Robot Configuration tool.

# vexcodeInit();

`vexcodeInit();` käytetään määrittämään ja alustamaan laitekonfiguraatiot Robotin konfigurointivälineellä. 

`The vexcodeInit();` on aina  "int main" funktion alussa varmistamaan, että laitteet on määritelty ennen muita komentoja.

Kos poistat tai laitat kommenteihin  `vexcodeInit();` kohdan aiheuttaa sen, etteivät laitteet toimi kunnolla ohjelmassasi.

<advanced>
</advanced>