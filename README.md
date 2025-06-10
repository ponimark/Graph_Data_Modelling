# 🕸️ Graph Data Modelling – NBA Player Relationship Analysis

This project explores graph-based data modeling using SQL to analyze relationships between NBA players, such as who played **with** or **against** each other, and how their performances compare over multiple games. It leverages the flexibility of graph structures to draw insights that are not easily achievable with traditional relational queries.

---

## 📁 Project Structure

| File Name              | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| `DDL.sql`              | Defines all required custom types and tables (vertices, edges, games, etc). |
| `vertices.sql`         | Populates the `vertices` table with player nodes, game nodes, etc.          |
| `edges.sql`            | Inserts relationships (e.g., `plays_with`, `plays_against`) into `edges`.   |
| `games_table.sql`      | Contains the raw schema and data for the `games` table.                     |
| `game_details_table.sql` | Schema and data for `game_details`, linking players to game stats.         |
| `final.sql`            | Final query combining data from vertices and edges to compare performance metrics like `points per game`, matchups, and collaborations. |

---

## 🧠 Key Concepts

- **Graph Database Design in SQL** using a `vertices` and `edges` structure
- **Modeling player interactions** such as:
  - `plays_with`
  - `plays_against`
- **Advanced aggregations** to compute:
  - Points per game
  - Performance against specific opponents
 

---

## 📊 Use Case

This modeling is ideal for:

- Sports analytics and recommendation systems
- Social graph-based insights
- Comparative performance metrics
- Understanding relationships in non-tabular structures

---

## 🚀 Getting Started

To run this project:

1. Load the schema via `DDL.sql`
2. Insert game and player data using:
   - `games_table.sql`
   - `game_details_table.sql`
3. Populate the graph:
   - `vertices.sql`
   - `edges.sql`
4. Run `final.sql` to view performance comparisons and relationship mappings.

---

## 📌 Example Output

The final output query allows insights such as:

- "Which players perform better when playing **against** certain players?"
- "What is the average performance when two specific players play **together**?"
- "Which players consistently outscore their opponents?"

---

## 🔧 Technologies Used

- PostgreSQL
- Window Functions
- Common Table Expressions (CTEs)
- JSON column handling
- Graph-style schema on relational database

---

## 📩 Contact

Developed by [@ponimark](https://github.com/ponimark)  
For questions or collaboration, feel free to open an issue or drop a message!

---

