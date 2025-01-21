# vio_intox  
Com base nos arquivos de exportação DBF gerados no SINAN NET, violência (Y09) e intoxicação exógena(T65.9), esse utilitário identifica casos notificados de violência classificados como envenenamento, porém, sem a devida notificação correspondente desse meio de agressão nos casos de intoxicação exógena registrados no SINAN.

Sintaxe do executável:

~~~
vio_intox.exe [municipio]

[municipio] Código IBGE do município de residência com 06 dígitos.

Exemplo: vio_intox 520620
~~~

Advertimos que o arquivo resultante do processamento poderá conter vários 
