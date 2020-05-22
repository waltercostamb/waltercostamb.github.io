---
layout: post
title: "Podcast IBICT: Material de Estudo de Pesquisa em Bioinformática"
date: 2020-05-22
---

Esse post surgiu da colaboração com as pesquisadoras Hetiene Pereira Marques e Joelma Fernanda Silva Carneiro do 
[Canal Ciência do IBICT](http://www.canalciencia.ibict.br/) (Instituto Brasileiro de Informação em Ciência e Tecnologia). 
A equipe do Canal Ciência está com um projeto super interessante de divulgação ciêntífica para estudantes de ensino 
fundamental e médio. Esse projeto consiste num [podcast](https://comunidade.rockcontent.com/o-que-e-podcast/), programa 
online em forma de áudio, sobre ciência com um convidado cientista.  

Nesse podcast conversaremos sobre a minha pesquisa dentro do campo da Bioinformática. Como eu sei que essa não é uma
área muito conhecida fora da academia, respondi alguns questionamentos básicos sobre Bioinfomática:

  - O que é Bioinformática?  
  
      Bioinformática é uma área relativamente nova da ciência, que aplica técnicas de ciência da computação, estatística e 
  matemática em problemas de natureza biológica.
  
  - Quem faz Bioinformática?  
  
      Bioinformática é uma área coloborativa por natureza. Bioinformatas são os profissionais mais tradicionais, que tiveram
  alguma formação formal (Graduação ou Pós-Graduação). Eles têm conhecimento de nível superior básico tanto em uma ou mais 
  áreas biológicas quanto em áreas básicas de exatas, como programação e lógica. Também trabalham em Bioinformática
  profissionais de áreas diferentes, mas afins, como biólogos computacionais ou teóricos, agrônomos, engenheiros florestais,
  cientistas ou engenheiros da computação, estatísticos, matemáticos e físicos, entre outros.
  
  - Para que serve essa Bioinformática?
  
      Essa ciência é fundamental atualmente. Com o desenvolvimento e barateanento de tecnologias de sequenciamento, a quantidade
  de dados biológicos disponível é absurda. Esses dados não pode ser analisados de formas tradicionais, e requerem técnicas
  robustas como a de programação. Em essência, a Bioinformática nos ajuda a melhor compreender qualquer sistema biológico
  que tenha disponíveis dados computacionais, como sequências.
  
  - Por que Bioinformática é importante?  
  
      Com um exemplo extremamente atual, temos a pandemia de COVID-19 (Coronavírus). Sem o sequenciamento rápido de genoma e sua
  análise, teria sido extremamente difícil e demorado entender como o vírus funciona, o que é fundamental para seu combate
  e controle. A Bioinformática em essência oferece suporte para biólogos e médicos, como no caso do coronavírus, e também
  para outras áreas, como exemplo, na melhoria de microorganismos para processamento de plantas de interesse comercial.
  
  - Quais habilidades pessoais e técnicas é preciso ter para ser um Bioinformata?  
  
      O Bioinformata é curioso e estudioso por natureza. É preciso também gostar de aprender, de colaborar com outras 
  pessoas e de aceitar as diferenças de outras áreas e de outros pesquisadores. Não é preciso uma habilidade natural 
  por ciência ou matemática, embora isso ajude. É possível aprender todo o necessário com esforço e persistência. Ter
  um ou mais mentores é também fundamental, já que seria extremamente difícil aprender essa ciência sozinho. Como comparação,
  é só imaginar aprender Biologia ou Computação sem um ou mais mentores.
  
  - Onde se pode aprender Bioinformática?  
  
      Até onde eu sei, não existe ainda nenhum curso superior, Bacharelado, em Bioinformática no Brasil. Existem porém diversos 
  cursos de pós-graduação strictu sensu de Mestrado e Doutorado voltados para essa área. Eu por exemplo, estudei 
  Biologia (Bacharelado) na graduação, fiz um projeto de iniciação científica em Bioinformática e depois cursei o Mestrado no
  Laboratório de Bioinformática do
  [Programa de Pós-Graduação em Biologia Molecular da Universidade de Brasília](https://www.ppgbiomol.com.br/pt/).
  
      Para aprender Bioinformática, eu sugiro o caminho mais tradicional que é o de estudar Bacharelado em Biologia ou Ciência
  da Computação, dependendo das suas inclinações pessoais. Se como eu, você é apaixonado por entender como a vida funciona,
  foque em Biologia primeiro. Mas se você gosta mais de matemática e lógica, siga primeiro na Ciência da Computação ou similares
  (como Engenharia da Computação ou até mesmo Estatística ou Matemática). Depois desse início no Bacharelado, você precisa se 
  especializar e aprender coisas da outra área. Para isso eu recomendo a Pós-Graduação (Mestrado ou Mestrado e Doutorado).

<img border="0" src="https://github.com/waltercostamb/waltercostamb.github.io/blob/master/figures/bioinformatica.png?raw=true" height="250" />   

**Pesquisa: SSS-test (Teste de Seleção de Estrutura Secundária)**

A bioinformática é uma área relativamente nova da ciência, que aplica o imenso poder de
processamento e análise da ciência da computação diretamente nos problemas existentes em ciências
biológicas. Como um exemplo bastante interessante, temos uma questão fundamental de biologia
evolutiva: quais determinantes genéticos nos diferenciam de espécies evolutivamente próximas, como
os chimpanzés? Para responder a essa pergunta podemos usar técnicas de bioinformática, associando
biologia e ciência da computação.

Mais detalhadamente, devemos estudar famílias de genes de primatas e descobrir quais genes
tem funções humano-específicas. Genes podem ser classificados em dois grandes grupos: proteínas e
RNAs não codificadores (ncRNAs). No nosso trabalho publicado na revista científica BMC
Bioinformatics em 2019, apresentamos o SSS-test (test for Selection on Secondary Structure), primeiro
programa da comunidade científica mundial capaz de analisar famílias de ncRNAs e reportar o grau
evolutivo correspondente para espécie. Com o SSS-test, analisamos 15 mil famílias de ncRNAs de
primatas e encontramos um pequeno grupo de 110 ncRNAs com sinais humano-específicos.

<img border="0" src="https://github.com/waltercostamb/waltercostamb.github.io/blob/master/figures/arvore.png?raw=true"  height="400" /> 

Como isso é feito? Primeiro, construímos um algoritmo teórico com os seguintes passos:  

  - (i) recebe como entrada os genes de ncRNAs;  
    
  - (ii) detecta as diferenças entre as espécies e   
    
  - (iii) constrói modelos estatísticos de impacto estrutural (com um impacto alto indicando função espécie-específica).  
    
Após definirmos esse novo algoritmo, eu o implementei por meio de uma linguagem de programação. Dessa forma, pude traduzir 
nossas ideias teóricas e fórmulas estatísticas numa linguagem que o computador entende e processa. 
  
Com o SSS-test, analisamos 15 mil famílias de ncRNAs de primatas e encontramos um pequeno grupo de 110 ncRNAs com sinais 
humano-específicos. Alguns deles estão ativos no nosso cérebro, o que pode levar a descobertas futuras ainda mais 
intrigantes. Dessa forma nós aumentamos nosso conhecimento sobre o que nos torna diferentes de outras espécies próximas, 
como os chimpanzés, ou, em outras palavras, o que exatamente nos torna humanos.

O SSS-test também pode ser usado para estudos evolutivos de outras espécies, tanto de mamíferos, quanto plantas ou fungos. 
Isso nos ajuda principalmente a entender como as espécies funcionam, o que é fundamental para o desenvolvimento científico e
é chamado de ciência básica. 

Referências:

Maria Beatriz Walter Costa, Christian Höner zu Siederdissen, Marko Dunjić, Peter Stadler, Katja Nowick. 
SSS-test: a novel test for detecting positive selection on RNA secondary structure. BMC Bioinformatics 20, 
151 (2019) https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2711-y

Katja Nowick, Maria Beatriz Walter Costa, Christian Höner zu Siederdissen, Peter Stadler. Selection Pressures 
on RNA Sequences and Structures. Evolutionary Bioinformatics Online. (2019)
https://journals.sagepub.com/doi/10.1177/1176934319871919

Maria Beatriz Walter Costa. Programa: SSS-test. (2019) https://github.com/waltercostamb/SSS-test


