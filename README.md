# vio_intox  
Com base nos arquivos de exportação DBF gerados no SINAN NET, violência (Y09) e intoxicação exógena(T65.9), esse utilitário identifica casos notificados de violência classificados como envenenamento, porém, sem a devida notificação correspondente desse meio de agressão nos casos de intoxicação exógena registrados no SINAN.

Sintaxe do executável:

~~~
vio_intox.exe [municipio]

[municipio] Código IBGE do município de residência com 06 dígitos.

Exemplo: vio_intox 520620
~~~

Advertimos que o arquivo resultante do processamento poderá conter falsos positivos, isto é, ocorrência de casos em que há notificações de intoxicação exógena no sistema relacionado aos casos notificados de violência por envenenamento. Isto ocorre devido à inconsistência dos dados trabalhados, por exemplo, durante o processamento de uma base, surgiu um caso de um mesmo paciente com três notificações diferentes e cada uma com um nome de mae diferente. Casos também com o mesmo paciente com notificações distintas com a data de nascimento diferente em cada notificação. Como o algoritmo trabalha com os campos que contêm o nome do paciente, data de nascimento e nome da mae do paciente, dados inconsistentes como os exemplificados, impedem que o processamento ocorra sem erros. Assim, sugerimos que se faça a verificação com o arquivo que foi gerado no processamento, se os casos apresentados têm, de fato, casos de intoxicação exógena registrados ou não no SINAN NET.



