# DioBank — TypeScript OOP

> Sistema bancário com TypeScript demonstrando os pilares de Orientação a Objetos: abstração, encapsulamento e herança.

## Arquitetura

```
DioAccount (abstract)
├── PeopleAccount   → conta pessoa física
└── CompanyAccount  → conta pessoa jurídica
```

## Conceitos aplicados

| Conceito | Implementação |
|---------|--------------|
| Classe abstrata | `DioAccount` não pode ser instanciada diretamente |
| Encapsulamento | `name` e `status` são `private` |
| `readonly` | `accountNumber` não pode ser reatribuído |
| Herança | `PeopleAccount` e `CompanyAccount` estendem `DioAccount` |
| Getters/Setters | `getName()` / `setName()` com validação de status |

## Stack

<img src="https://skillicons.dev/icons?i=ts,nodejs" />

## Como rodar

```bash
npm install
npm run dev
```

## Exemplo

```typescript
const conta = new PeopleAccount(1, "Ygor", 10)
conta.deposit()   // Voce depositou
conta.withdraw()  // Voce sacou
conta.getBalance()
```

---

Desenvolvido com TypeScript · Programação Orientada a Objetos