# PROJETO: Loja Virtual Clean Architecture + DDD (Pure PHP)
**STATUS ATUAL**:
✅ Repositório Git criado  
✅ composer.json configurado com:
  - MongoDB driver  
  - Swagger docs  
  - PSR-4 autoload (namespace Cleanstore\Kkg)  
✅ Estrutura básica de pastas criada  

**PRÓXIMOS PASSOS CRÍTICOS**:
1. [ ] Instalar e configurar MongoDB localmente
2. [ ] Criar entidade `Produto` em `src/Domain/Entities/`
3. [ ] Implementar `ProdutoRepositoryInterface` 
4. [ ] Criar caso de uso `CadastrarProduto`
5. [ ] Configurar container DI para injeção de dependências
6. [ ] Implementar endpoint API em `public/index.php`

**COMANDOS PARA CONTINUAR**:
```bash
# 1. Instalar MongoDB (Linux/macOS)
sudo apt-get install mongodb-community  # ou brew para Mac

# 2. Iniciar serviço MongoDB
sudo systemctl start mongod

# 3. Criar primeira entidade
touch src/Domain/Entities/Produto.php

# 4. Rodar projeto (após implementações)
docker-compose up -d