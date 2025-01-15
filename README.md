# E-commerce-projeto-conceitual
Refinamento de um projeto conceitual de um E-commerce da DIO
# Descrição
Cliente PJ e PF: Cada conta é definida como Pessoa Física (PF) ou Pessoa Jurídica (PJ), garantindo exclusividade.
Pagamento: Relacionamento que permite múltiplas formas de pagamento.
Entrega: Contém atributos como status e código de rastreio.
# Restrições e Relacionamentos:
Cliente → Pessoa Física e Pessoa Jurídica: Cada cliente terá exatamente uma das duas tabelas associadas (exclusividade via lógica de aplicação ou triggers).
Cliente → Pagamento: Relacionamento de 1 para N, onde um cliente pode ter várias formas de pagamento.
Pedido → Entrega: Relacionamento 1 para 1, cada pedido possui uma entrega.
# Descrição das Conexões:
Cliente ↔ Pessoa_Física / Pessoa_Jurídica: Relacionamento exclusivo de 1 para 0 ou 1.
Cliente ↔ Pagamento: Um cliente pode ter várias formas de pagamento (1 para N).
Cliente ↔ Pedido: Um cliente pode realizar vários pedidos (1 para N).
Pedido ↔ Entrega: Cada pedido tem exatamente uma entrega (1 para 1)
