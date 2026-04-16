Porque secret é tratada como informação sensível. A ferramenta esconde automaticamente o valor nos logs pra evitar que alguém veja sem querer. Por isso aparece como ***.
Já uma variável comum não tem essa proteção, então o valor dela aparece normalmente.


Na maioria dos casos, não.
Cada job roda separado, como se fosse um ambiente novo. Então o que você cria dentro de um job não vai automaticamente pro outro.
Se quiser usar essa variável no Job 2, precisa passar ela de forma explícita, tipo usando output do job ou algum outro mecanismo da ferramenta.
