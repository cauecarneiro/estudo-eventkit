# Estudo de EventKit

Estudo do EventKit em SwiftUI: adicionar eventos ao Calendário do iPhone a partir de um app.

Estudo · iOS 26 · 2025

## O que faz
- Lista dois eventos de exemplo, com data.
- Ao tocar num evento, pede acesso ao Calendário e cria o evento de 1 hora no calendário padrão do aparelho.
- Mostra um alerta de sucesso ou de erro (inclusive quando o acesso é negado).

## Meu papel
Estudo solo. Todos os commits são meus.

## Como foi feito
- Tudo em `ContentView.swift`.
- Usa `requestWriteOnlyAccessToEvents`, o acesso só de escrita: o app grava no calendário sem poder ler os eventos do usuário.
- O evento é um `EKEvent` com título, data, duração de uma hora e notas, salvo em `defaultCalendarForNewEvents`.
- O projeto declara as chaves de uso do Calendário (`NSCalendarsUsageDescription` e `NSCalendarsWriteOnlyAccessUsageDescription`).

## Tecnologias
Swift, SwiftUI e EventKit.

## Como rodar
1. Abra `EventKitApp/EventKitApp.xcodeproj` no Xcode.
2. Rode num simulador com iOS 26 ou mais novo, toque num evento e permita o acesso ao Calendário.

---
Feito por Cauê Crillanovick · [portfólio](https://cauecarneiro.github.io/portfolio/) · [LinkedIn](https://www.linkedin.com/in/cau%C3%AA-carneiro)
