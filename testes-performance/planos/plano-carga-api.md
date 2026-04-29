# Plano de Teste de Performance — API de E-commerce

## Objetivo
Validar o comportamento da API sob carga de **100 usuários simultâneos**, identificando gargalos e limites de capacidade.

## Escopo
| Endpoint | Método | Cenário |
|----------|--------|---------|
| `/api/produtos` | GET | Listagem de produtos |
| `/api/login` | POST | Autenticação de usuários |
| `/api/carrinho` | POST | Adição de item ao carrinho |

## Critérios de aceite
| Métrica | Meta |
|---------|------|
| Tempo de resposta médio | < 2 segundos |
| Percentil 95 (P95) | < 4 segundos |
| Taxa de erro | < 1% |
| Throughput | > 50 req/s |

## Cenários de teste

### Cenário 1 — Carga gradual (Ramp-up)
- Início: 0 usuários
- Crescimento: +10 usuários a cada 30s
- Pico: 100 usuários simultâneos
- Duração no pico: 5 minutos

### Cenário 2 — Carga constante
- Usuários: 50 simultâneos
- Duração: 10 minutos

### Cenário 3 — Pico repentino (Spike)
- Base: 10 usuários
- Pico: 200 usuários por 1 minuto
- Retorno à base

## Ferramentas
- **JMeter 5.x** — execução dos testes
- **GitHub** — versionamento dos scripts

## Ambiente
- Ambiente: Homologação
- URL base: `https://api-homolog.exemplo.com`
