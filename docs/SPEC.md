# family-budget: Global specification

Status: Draft

## 1. Functional

### 1.1 General description

A modular, mobile-first PWA for managing a family's budget and finances: tracking expenses and investments,
and planning a budget.

### 1.2 Module families

The app is made of modules, in two families:

1. **Data modules:** they bring data into the app and let users manage it (import, enter, edit).
2. **Analysis modules:** they use the data from the data modules. Each analysis module declares which data it needs
   from the user to work correctly. _To be defined later._

### 1.3 Data modules

| Module | Description |
|---|---|
| Investment tracking | Tracks investments. Tracking only: no trading from the app. Data comes in through import sources. The first source is Wealthsimple export files. Others (an API, for example) may come later, so adding an import source must be easy and must not require changes to the rest of the module. |
| Expense tracking | Imports bank account and credit card statements and processes them. Each expense is assigned a category, so analysis modules can use it later. |
| Budget planning | Users build a budget that allocates money to buckets such as investments, fixed costs, restaurants and leisure. _Details to come._ |
| Mortgage | Users enter their mortgage and its conditions. Must support Canadian portable ("moving") mortgages and variable rates. |

Each data module will get its own spec in `docs/specs/`.

## 2. Technical

_To be defined together._

## 3. Ground rules

_To be defined together._

## 4. Modules

Each module gets its own spec file in `docs/specs/`. None defined yet.
