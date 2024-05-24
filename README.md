## Entidades de Domínio:

1. **Produto:**  Cada produto no estoque é uma entidade. Cada produto tem um número de identificação único e pode ter informações adicionais como tamanho e cor.
  
  - *Atributos:*

    - ID único
    - Nome
    - Quantidade em estoque
    - Quantidade mínima
    - Tamanho
    - Cor
    - Preço

        
2. **Estoque:** O estoque é onde os produtos são armazenados. Cada produto no estoque tem uma quantidade associada a ele.

  - *Atributos:*
    
    - Produto
    - Quantidade atual
    - Histórico de movimentações


3. **Alerta:** Um alerta é gerado quando a quantidade de um produto no estoque cai abaixo de um limite mínimo definido.

  - *Atributos:*
    
    - Tipo de alerta (e-mail, notificação)
    - Mensagem
    - Destinatário

4. **Histórico de Vendas:** O histórico de vendas registra a quantidade de produtos vendidos em um determinado período, o lucro gerado por produto e quais produtos estão vendendo melhor em cada período.

  - *Atributos:*
    
    - ID da venda
    - Data
    - Produto(s) vendido(s)
    - Quantidade
    - Preço total
    - Lucro gerado

5. **Ordem de Compra:** Uma ordem de compra é criada quando é necessário reabastecer o estoque. As ordens de compra são geradas automaticamente com base nas quantidades mínimas de estoque definidas e nas tendências de vendas.

  - *Atributos:*
    
    - ID da ordem
    - Produto(s) a ser(em) comprado(s)
    - Quantidade
    - Data de criação
    - Status (pendente, concluída, etc.)
    - Prazo de entrega
    - Fornecedor


6. **Fornecedor:** O fornecedor fornece os produtos que são armazenados no estoque.

  - *Atributos:*
    
    - ID do fornecedor
    - Nome
    - Contato
    - Produtos fornecidos
    - Prazos de entrega

## Casos de Uso:

1. **Rastrear Produto:** Atribuir um número de identificação único a cada produto, adicionar e atualizar informações do produto e rastrear suas movimentações no estoque.

2. **Definir Quantidades Mínimas de Estoque:** Definir um limite mínimo para cada produto no estoque e atualizar limites mínimos conforme necessário.

3. **Receber Alertas**: Receber alertas por e-mail e por meio de uma notificação no sistema de gerenciamento de estoque quando a quantidade de um produto no estoque está próxima do fim e configurar preferências de alerta.

4. **Visualizar Histórico de Vendas e Estoque:** Visualizar quantos produtos foram vendidos em um determinado período, qual foi o lucro gerado por produto, quais produtos estão vendendo melhor em cada período, monitorar as tendências de estoque ao longo do tempo e analisar tendências para suportar decisões de compra.

5. **Criar e Gerenciar Ordens de Compra:** Criar e gerenciar ordens de compra automaticamente com base nas quantidades mínimas de estoque definidas e nas tendências de vendas,
atualizar status das ordens de compra e integrar com fornecedores para atualizações automáticas.

6. **Integrar com Fornecedores:** Integrar o sistema com os fornecedores para receber atualizações automáticas sobre os prazos de entrega de novas remessas.
