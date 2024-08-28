# Predicao_de_Cancer_Modelos_ML

A oncologia está cada vez mais integrada com a ciência dos dados, permitindo avanços significativos no diagnóstico e tratamento de cânceres. Um dos desafios mais críticos enfrentados pelos médicos é a determinação precisa da natureza de um tumor, ou seja, se ele é benigno ou maligno. Essa distinção é importante para o planejamento do tratamento e para as chances de recuperação do paciente.

Para esse artigo, utilizei uma base de dados de diagnóstico de câncer de mama do estado de Wisconsin nos EUA para desenvolver um modelo preditivo que auxilia na classificação de tumores. Por meio de técnicas de machine learning, é possível identificar padrões sutis que diferenciam as características benignas das malignas, oferecendo uma ferramenta adicional para os médicos na tomada de decisões.

A aplicação dessas metodologias não só aprimora a precisão dos diagnósticos, mas também acelera o processo, permitindo intervenções mais rápidas e personalizadas. Este artigo explora apenas o processo de desenvolvimento do modelo preditivo, discutindo a escolha das métricas que influenciam a análise. 

Para realizar uma predição eficaz de câncer de mama, utilizei 4 algoritmos de machine learning, são eles:

* Decision Tree;
* Regressão Logística;
* Random Forest;
* LightGBM.

O que determina a qualidade do modelo são as métricas. A escolha das métricas a serem priorizadas dependerá do contexto clínico específico e dos riscos associados a falsos positivos e falsos negativos. Sendo assim, destaquei duas importantes métricas, Precision e Recall.

O Precision mede a proporção de verdadeiros positivos ( tumores corretamente identificados como malignos) entre todas as predições positivas (verdadeiros positivos + falsos positivos). Ela é importante quando o custo de um falso positivo é alto, ou seja, quando classificar incorretamente um tumor benigno como maligno pode levar a tratamentos desnecessários. 

O Recall mede a proporção de verdadeiros positivos identificados entre todos os casos reais de malignidade (verdadeiros positivos + falsos negativos). Essa métrica é fundamental quando o custo de um falso negativo é alto, como em casos onde deixar de identificar um tumor maligno pode ter consequências graves.

Entre os quatro algoritmos testados, o Random Forest apresentou o melhor desempenho em termos das métricas. O Precision alto de 98% assegura que a maioria das predições de malignidade estejam corretas, enquanto um Recall elevado com 95% garante que a maioria dos casos malignos sejam corretamente identificados. O Random Forest se destacou por sua capacidade de equilibrar essas duas métricas, proporcionando um modelo confiável para a predição da natureza dos tumores. 

O gráfico da curva Precision-Recall mostra que o desempenho no treino é refletido quase que perfeitamente no teste, o que é um indicativo de que o modelo será robusto ao ser aplicado em dados novos.

Com o modelo ajustado, o impacto na assertividade no diagnóstico irá permitir que os médicos definam o tratamento mais adequado para o paciente. Se o tumor for benigno, tratamentos invasivos e desnecessários podem ser evitados. Se for maligno, um diagnóstico preciso garante que o tratamento seja iniciado rapidamente, aumentando as chances de sucesso.

Para os pacientes, receber um diagnóstico preciso é fundamental para reduzir a ansiedade e o estresse associados à incerteza. Saber exatamente a natureza do tumor ajuda a tranquilizar o paciente ou a prepará-lo mentalmente para os próximos passos do tratamento.

Por fim, a assertividade no diagnóstico do câncer de mama é essencial para garantir que os pacientes recebam o tratamento certo no momento certo, melhorando assim as taxas de cura e a qualidade de vida.



