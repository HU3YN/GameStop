# GameStop Retail Interface

A Java console app that runs a GameStop-style store: a game catalog, customer and employee accounts, and orders, with separate Manager, Employee and Customer roles. It was a six-person team project for CIS 22C (Data Structures) at De Anza College, Mar 2025. This is my fork of the team repository. The interface is terminal-only.

**My part:** I wrote the Employee class and about a third of the main interface, planned the layout with the team (which structure holds which data, the order flow and the menus), and wrote this README. The team worked on the data structures together.

## Data structures

- **Binary search trees:** two trees hold the games, one sorted by title (TitleComparator) and one by genre (GenreComparator). They are built to minimal height, so search is O(log n).
- **Hash table:** holds customer accounts for fast login lookups.
- **Heap:** orders unshipped orders by shipping priority (Standard, Rush, Overnight).
- **Linked lists:** track each customer's shipped orders.

## Features

- Search the catalog by title, or view games by genre.
- Customers place orders. Employees can search orders by ID or customer name, view the highest-priority order, view all orders and ship an order.
- All changes (inventory, orders, accounts) are saved to local text files when the program exits.

About 3,800 lines of Java. The team used scrum meetings and sprints, user stories and a product backlog.
