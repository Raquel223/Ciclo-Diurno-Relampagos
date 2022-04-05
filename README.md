# Ciclo Diurno Relâmpagos

### Ciclo diurno dos relâmpagos das redes de detecção BrasilDAT e SPLMA, obtidos durante a campanha CHUVA-Vale do Paraíba, que ocorreu entre novembro de 2011 e março de 2012.

---

> **BrasilDAT**


**Descrição do dado bruto (a quantidade de linhas e colunas correspondem a junção de todos os arquivos dentro do arquivo .tar):**


| Propriedade                        | Descrição   |
| :--------------------------------- |:------------|
| Rede de detecção                   | BrasilDAT   |
| Arquivo                            | 2_dezembro.tar.gz |
| Linhas                             | 3569936         |
| Colunas                            | 14  |

Após filtrar somente as colunas que serão utilizadas e somente os relâmpagos cuja distância (centro da SPLMA e coordenada do relâmpago) é igual ou menor que 100 km:


| Propriedade                        | Descrição   |
| :--------------------------------- |:------------|
| Rede de detecção                   | BrasilDAT   |
| Arquivo                            | Novo_Dezembro.csv |
| Linhas                             | 241263         |
| Colunas                            | 9 |

Para gerar o arquivo acima **Novo_Dezembro.csv**, é necessário rodar o código **Tabela_distancia_BrasilDAT.ipynb**.

A partir de agora, com o arquivo Novo_Dezembro.csv, poderão ser geradas as seguintes figuras:

* **Ciclo diurno da frequência de relâmpagos** (Frequência_BrasilDAT_Dezembro.ipynb);
* **Pico de corrente** (pico_corrente_BrasilDAT.ipynb);
* **Evolução da ocorrência ao longo do mês de relâmpagos do tipo IC** (IC_Gráfico_por_dia_BrasilDAT.ipynb).

Lembrando que para estes exemplos, foram utilizados dados do mês de dezembro de 2011. 

---


> **SPLMA**

**Descrição do dado bruto (a quantidade de linhas e colunas correspondem a junção de todos os arquivos dentro do arquivo .tar)**:


| Propriedade                        | Descrição   |
| :--------------------------------- |:------------|
| Rede de detecção                   | SPLMA   |
| Arquivo                            | 2011-11_pasta1_v01.tar.gz |
| Linhas                             | 44346         |
| Colunas                            | 13  |

Para os dados da SPLMA, primeiramente é necessário organizar o dado por exemplo:

* Renomear as colunas de todos os arquivos
* Descobrir o número de fontes de cada arquivo
* Pegar somente a primeira linha de cada arquivo
* Inserir uma coluna para cada arquivo

Após organizar o dado e filtrar somente os relâmpagos cuja distância (centro da SPLMA e coordenada do relâmpago) é igual ou menor que 100 km:

| Propriedade                        | Descrição   |
| :--------------------------------- |:------------|
| Rede de detecção                   | SPLMA   |
| Arquivo                            | Novembro_100km.csv |
| Linhas                             | 38412          |
| Colunas                            | 14 |


Para gerar o arquivo acima **Novembro_100km.csv**, é necessário rodar o código **organizar_dado_distância_SPLMA.ipynb**.

A partir de agora, com o arquivo Novembro_100km.csv, poderá ser gerada a seguinte figura **Ciclo diurno dos relâmpagos** (Ciclo_diurno_SPLMA.ipynb) as quais serão analisadas as variáveis: 

* **Frequência**;
* **Altura**;
* **Fontes**;
* **Comprimento**;
* **Duração**.

Lembrando que para estes exemplos, foram utilizados dados do mês de novembro de 2011.

