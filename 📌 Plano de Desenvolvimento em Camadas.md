📌 Plano de Desenvolvimento em Camadas
1. Domínio (Core Business)
Entidades:

Produto (id, nome, preço, estoque, categorias)

Usuario (id, email, senha hash, perfil)

Carrinho (id, itens, usuário_id)

Pedido (id, itens, status, valor_total)

Serviços de Domínio:

CalculadoraFrete

ValidadorEstoque

ProcessadorPagamentos (integração com Banco do Brasil)

2. Aplicação (Casos de Uso)
Funcionalidade	Caso de Uso
Catálogo	ListarProdutosDisponiveis
Admin/CRUD	CadastrarProduto
Carrinho	AdicionarItemAoCarrinho
Checkout	FinalizarPedido
Pagamento	VerificarPagamentoPix
3. Infraestrutura
Banco de Dados:

MongoDB para produtos/carrinhos

MySQL para usuários/pedidos (por transações ACID)

APIs Externas:

API Pagamentos Banco do Brasil (PIX)

ViaCEP (validação de endereço)