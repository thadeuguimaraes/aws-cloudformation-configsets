# Configsets 

- Podemos criar mais de uma chave de configuração e ter um processo de entrada CFN
eles em uma ordem específica.
  - Configset único
  - Múltiplo Configset

# Step#1: Single Configset

# Vamos definir duas chaves de configuração App1 e App2
## Vamos criar um conjunto de configurações com o nome como
## App1 and App2.
- A chave de configuração do primeiro App1 será executada.
- Próxima chave de configuração do App2 será executada.
- A ordem de execução será baseada em como
Nós os definimos em configurações.
- Observação
  - Ambas as aplicações devem estar acessíveis

# Step#2: Multiple configSets

## Criamos 3 configurações
  - SingleAppcs
  - DualAppcs
  - default
- SingleAppcs: apenas App1 deve ser
implantado.

# Step#3: Multiple configSets

## Criamos 3 configurações
  - SingleAppcs
  - DualAppcs
  - default
- DualAppcs: App1 e App2 devem
ser implantado
 
 # Step#4: Multiple configSets

## Criamos 3 configurações
  - SingleAppcs
  - DualAppcs
  - default
- Default: o default contém o ConfigSet
Dualappcs para que ambos os aplicativos devem ser
implantado.Por padrão, não precisamos
especificar "-Configsets default", ele escolherá
automaticamente.
