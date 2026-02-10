# RCR

# Edição de teste para a IA revisar
calcular_media <- function(dados) {
  
  # ERRO 1: Loop for lento (IA vai sugerir vetorização)
  resultado <- 0
  for (i in 1:length(dados)) {
    resultado <- resultado + dados[i]
  }
  
  # ERRO 2: Divisão perigosa (Pode gerar erro se o vetor estiver vazio)
  media <- resultado / length(dados)
  
  # ERRO 3: Falta de tratamento de NA (Se houver um NA, o resultado será NA)
  return(media)
}

# Teste com erro
meus_dados <- c(10, 20, NA)
print(calcular_media(meus_dados))
