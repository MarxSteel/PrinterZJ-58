zj-58
=====
Filtro CUPS para impressora térmica Zjiang ZJ-58

O driver linux fornecido no site Zjiang infelizmente não funciona. Primeiro, é um binário de 32 bits (e, portanto, no sistema x64, é necessário instalar algumas bibliotecas x86). Segundo, o PPD não está correto - ele simplesmente não mostra configurações avançadas por causa disso. Finalmente, o filtro raster apenas trava em qualquer tentativa de executá-lo! Mas mesmo se você executá-lo, você verá que ele está funcionando com a impressora não é ideal: por exemplo, se ele vir uma linha em branco, ele enviará a rasterização em branco para imprimir (em vez de usar o comando 'feeding', que é definitivamente mais rápido!)

Esta é a solução: o PPD é fixo e funciona. O filtro é fornecido como src (você pode encontrar uma lista de pacotes que precisam ser instalados para construí-lo no cabeçalho da origem). Além disso, a impressão de linhas em branco é otimizada.
