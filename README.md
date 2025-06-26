# Aviso

Deixando claro: o conteúdo abaixo veio de um curso gratuito e não pode ser redistribuído. Se quiser estudar o assunto, procure o curso aberto da trilha de Java com Spring Boot. Se a plataforma fechar o acesso ou passar a cobrar, não está no meu alcance — mas o material é muito bom e quem assina um plano alcança bem mais.


### Side note

A ordem dos passos importa: nao pule a preparacao do ambiente.

---

Experimento com interfaces. A ideia não é testar o óbvio: basta abrir os arquivos para entender. Eu crio uma instância declarando o tipo como o de uma interface.

Um ponto curioso é a visibilidade dos métodos de uma interface: tentar marcar um método da interface como **protected** faz o editor acusar erro, dizendo que só são permitidos os modificadores public, abstract, default, static e strictfp.

Pontos de atenção:

- num método de interface ele é obrigatoriamente abstrato, sem implementação;
- numa classe base o método pode ter implementação;
- o método de interface pode ser público, abstrato, padrão ou estático; não pode ser privado nem protegido;
- na herança, o que não se pode é reduzir a visibilidade de um método, nem trocar o tipo de retorno;
- quanto aos parâmetros, na herança dá para mudar o tipo de um parâmetro, mas com interfaces não.

Sobre atributos em interfaces, existe uma resposta pública explicando que eles podem existir, mas não funcionam como se espera: são tratados como constantes estáticas.

Repare que numa das interfaces criei um atributo constante.