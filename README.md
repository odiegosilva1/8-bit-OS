# SAP-1 (SIMPLE AS A POSSIBLE) COMPUTER 


1 - Programa Armazenado (strong-program)
  
  No SAP-1, todas as instruções (opecodes) quanto os dados (operandos) residem
  na RAM de 16 bits, sem distribuição física entre eles.

2 - barramento único para dados e instruções.

  O barramento de dados (W Bus) é compartilhado para trafegar a instruções buscando na RAM e,
  no ciclo seguinte, o dado a ser processado. Isso reproduz fielmente o famoso "Gargalo de Von      Neumann" (a contenção no barramento), onde a CPU fica limitada pela velocidade de transferência   entre a memória e o processador.

3 - Ciclo Busca-Decodifica-Executa (Fetch-Decode-Execute)

  A unidade de controle do SAP-1 é síncrona e sequencial. Primeiro, ela ativa o fetch, estágio em   que busca a instruções da RAM, no endereço designado pelo contador de programa, e a envia para    o registrador de instruções, depois decodifica o opcode e,  por fim, executa a instrução.
