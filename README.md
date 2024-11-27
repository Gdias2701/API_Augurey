# Augurey API 

<p align="justify">
  
A **Augurey API** classifica os estágios de degradação de componentes mecânicos baseando-se em dados de vibração. Seu objetivo é auxiliar na manutenção preditiva, prevenindo falhas catastróficas.
</p>

---
## Motivação
![Augurey](images/image.png)

<p align="justify">
  
O nome **Augurey** refere-se a uma ave que prenuncia mudanças iminentes, assim como a API alerta sobre o progresso da degradação de componentes mecânicos. O objetivo não é apenas prever o fim da vida útil, mas preparar a equipe de manutenção para agir preventivamente e evitar falhas em sistemas associados.
</p>

---

## Índice  
- [Descrição Geral](#descrição-geral)  
- [Como Usar](#como-usar)  
- [Detalhes dos Resultados](#detalhes-dos-resultados)  
- [Exemplo Prático](#exemplo-prático)  
- [Motivação](#motivação)  
- [Referências](#referências)  

---

## Descrição Geral  
A API utiliza como entrada:  
1. **Frequência de coleta** (em Hz).  
2. **Intervalo entre coletas** (em segundos).  
3. **Tamanho da janela de coleta** (em segundos).  
4. **Arquivos CSV contendo séries temporais de vibração** (vertical e horizontal).  

**Saída**: Classificação em 4 estágios de degradação com análise detalhada e gráficos evolutivos.

---

## Como Usar

### Passo 1: Inserir Parâmetros de Coleta
- Frequência: Exemplo `25600 Hz`.  
- Intervalo: Exemplo `10 s`.  
- Tamanho da janela: Exemplo `0,10 s`.

### Passo 2: Enviar Arquivos CSV
- Arquivo vertical: Exemplo `FEMTO_Test_B33V.csv`.  
- Arquivo horizontal: Exemplo `FEMTO_Test_B33.csv`.  
- **Tamanho máximo por arquivo**: 200 MB.  

### Passo 3: Processar os Dados
1. Clique em **Submit**.  
2. A API processará os dados e exibirá os resultados de análise.

---

## Detalhes dos Resultados

### Estágios de Degradação
- **Estágio 0**: Normal.  
- **Estágio 1**: Pequena degradação.  
- **Estágio 2**: Degradação intermediária.  
- **Estágio 3**: Grave (ação corretiva urgente).  

### Informações Fornecidas
1. **Tempo em cada estágio**:
   - Exemplo: Estágio 1 -> `21 minutos`.  
2. **Intervalos de tempo por estágio**:
   - Exemplo: Estágio 0 -> `Início: 0h, Fim: 3min`.  
3. **Estágio atual e probabilidade**:
   - Exemplo: Estágio 3 com 90% de probabilidade.  
4. **Gráfico evolutivo da degradação**.  

---

## Exemplo Prático

### Configuração de Entrada
- Frequência: `25600 Hz`.  
- Intervalo: `10 s`.  
- Janela: `0,10 s`.  
- Arquivos:
  - Vertical: `FEMTO_Test_B33V.csv`.  
  - Horizontal: `FEMTO_Test_B33.csv`.  

### Resultado
- **Estágio Atual**: 3.  
- **Probabilidade**: 90%.  
- **Tempo em Estágio 3**: 16 minutos.  
- **Ação Requerida**: Manutenção corretiva imediata.

---

## Referências
[1] Tianwen Zhu, Yongyi Ran, Xin Zhou, and Yonggang Wen, \textit{A Survey of Predictive Maintenance: Systems, Purposes and Approaches}, arXiv preprint arXiv:1912.07383, 2024. doi: \url{https://doi.org/10.48550/arXiv.1912.07383}.

[2] Nie, L., Zhang, L., Xu, S., and others, "Remaining useful life prediction for rolling bearings based on similarity feature fusion and convolutional neural network", Journal of the Brazilian Society of Mechanical Sciences and Engineering, vol. 44, pp. 328, 2022, doi: 10.1007/s40430-022-03638-0.

[3] C.~Scheffer and P.~Girdhar, \emph{Practical Machinery Vibration Analysis and Predictive Maintenance}. Elsevier, 2004.

[4] Juodelyte, D., Cheplygina, V., Graversen, T., and Bonnet, P., "Predicting Bearings' Degradation Stages for Predictive Maintenance in the Pharmaceutical Industry", 2022, doi: \url{
https://doi.org/10.48550/arXiv.2203.03259}.

[5] Ba he ti bie ke A LI QIE KE, Qing HUANG, Liang TIAN, Liwei ZHANG, and Kun WANG, "Fault Detection For Equipment in Distribution Grid Station House Based on Ubiquitous Internet of Things," \textit{IEEE Xplore}, 2024. Accessed on: 2024-09-24.

[6] Massaro, A., Manfredonia, I., Galiano, A., Pellicani, L., \& Birardi, V. (2019). Sensing and Quality Monitoring Facilities Designed for Pasta Industry Including Traceability, Image Vision and Predictive Maintenance. \textit{2019 II Workshop on Metrology for Industry 4.0 and IoT (MetroInd4.0\&IoT)}. doi: 10.1109/metroi4.2019.8792912.

[7] IEEE PHM 2012 Prognostic Challenge. Outline, Experiments, Scoring of Results, Winners, year={2012}, organization={IEEE}, url={https://pt.scribd.com/document/344094074/IEEEPHM2012-Challenge-Details-Results-and-Winners}

[8] Nectoux, P., Gouriveau, R., Medjaher, K., Ramasso, E., Chebel-Morello, B., Zerhouni, N., and Varnier, C., "PRONOSTIA: An Experimental Platform for Bearings Accelerated Degradation Tests", IEEE International Conference on Prognostics and Health Management (PHM), pp. 1--8, 2012.

[9] Iunusova, E., Gonzalez, M. K., Szipka, K., and Archenti, A., "Early fault diagnosis in rolling element bearings: Comparative analysis of a knowledge-based and a data-driven approach", Journal of Intelligent Manufacturing, vol. 35, pp. 2327--2347, 2024, Springer, doi: 10.1007/s10845-023-02151-y.

[10] M. Barandas, D. Folgado, L. Fernandes, S. Santos, M. Abreu, P. Bota, H. Liu, T. Schultz, and H. Gamboa,  "TSFEL: Time Series Feature Extraction Library," \textit{SoftwareX}, vol. 11, p. 100456, 2020.  DOI: 10.1016/j.softx.2020.100456. Accessed on: 2024-11-22.

---
- [Inspiração no Augurey (Harry Potter Wiki)](https://harrypotter.fandom.com/wiki/Augurey)

Pronto para implementação e análise com **Augurey API**! 🎉 Se tiver dúvidas, abra uma *issue*. 😊
