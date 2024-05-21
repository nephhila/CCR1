REATOR BATELADA - CINÉTICA E CÁLCULO DE REATORES 🧪

🔹CÓDIGO #1 - REAÇÃO ELEMENTAR DE PRIMEIRA ORDEM

📌 INTRODUÇÃO 📌

Este código realiza a simulação de uma reação de primeira ordem do tipo aA→bB. Ele calcula e plota as concentrações do reagente (A) e do produto (B) ao longo do tempo, além de fornecer uma opção para verificar a conversão do reagente em um ponto específico do tempo. O objetivo é que ele seja versátil e simples justamente para que possa ser alterado conforme as necessidades da empresa e/ou do usuário.

#️⃣ O MÉTODO NUMÉRICO #️⃣

O método numérico empregado para calcular a concentração do reagente A ao longo do tempo é a solução analítica da equação diferencial de uma reação de primeira ordem, que assume forma d[A]/dt = -k[A]. A solução desta ED é:

A = [A]_0 * exp(-kt)

Onde:

A é a concentração do reagente A no tempo t,
[A]_0 é a concentração inicial do reagente,
k é a constante de velocidade da reação,
t é o tempo.

O método analítico é muito útil para reações de primeira ordem e não requer a utilização de métodos mais complexos.

▶️ FUNCIONALIDADE DO CÓDIGO ▶️

 1. Funções de cálculo das concentrações:

	> concentracao_reagente(c0, k, t): Calcula a concentração do reagente A em um determinado tempo t. A fórmula utilizada é A = [A]_0 * exp(-kt), onde [A]_0 é a concentração inicial do reagente e k é a constante de velocidade da reação.
	> concentracao_produto(c0, k, t): Calcula a concentração do produto B em um determinado tempo t. Considera-se que toda a concentração inicial do reagente A eventualmente se converterá em B, logo, a concentração de B é dada por B = [A]_0 - A.

 2. Interação com o usuário:

	> O usuário é solicitado a fornecer a concentração inicial do reagente ([A]_0), a constante de velocidade da reação (k) e o tempo final da simulação.
	> Uma seção opcional permite ao usuário verificar a conversão do reagente em um ponto específico no tempo. A conversão é calculada como Conversão = (1 - A/[A]_0) * 100.

 3. Simulação e Plotagem:

	> Para simular a evolução da reação ao longo do tempo, o intervalo de tempo total é discretizado em 100 pontos usando a função np.linspace do numpy. Este método de discretização é uma técnica numérica básica que divide um intervalo contínuo em pequenos segmentos para facilitar o cálculo.
	> As concentrações de A e B são calculadas para cada ponto no tempo utilizando as funções definidas.
	> Duas figuras são geradas usando matplotlib:
		* A primeira figura mostra as concentrações de A e B ao longo do tempo.
	 	* A segunda figura mostra a conversão do reagente A ao longo do tempo.

💻 TECNOLOGIAS UTILIZADAS 💻 

 * Python (3.10.12)
 * Google Collab

🧑‍🔬 AUTORES 🧑‍🔬

 * DIMI FOGAÇA CANTELLI
 * GLEICI EVELLIN DE OLIVEIRA
 * PATRÍCIA LOUISE DA SILVA FERREIRA
 * TAINARA ADRIELE SCHUENKE

🔗 ACESSO AO PROJETO 🔗

