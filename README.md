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

