# Quitanda da Esquina
## 1. Liste pelo menos 4 problemas arquiteturais que você encontrou no código inicial e explique por que cada um viola o padrão MVC.
- Classe Produto estava no app.py.
- As rotas estavam todas no app.py.
- O HTML estava misturado com o Controller.
- O Blueprint de produtos não estava registrado.
- Havia código repetido para buscar produtos.
## 2. Onde ficou a camada Model no seu projeto? Onde ficaram os Controllers? Cite um trecho de cada.
- Model: ficou no arquivo models.py.
- A classe Produto ficou em models.py.
- Controller de produtos: blueprints/produtos/routes.py.
- Controller de autenticação: blueprints/auth/routes.py.
## Por que o url_for e os endpoints precisaram ser ajustados durante a refatoração? Cite um exemplo de mudança que você fez.
- Os endpoints mudaram porque as rotas passaram a usar Blueprints.
- Antes: url_for("index")
- Depois: url_for("produtos.index")
- Antes: url_for("logout")
- Depois: url_for("auth.logout")

