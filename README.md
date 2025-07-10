# pokemon-damage-simulator
## 📌 Project Overview
This project is part of a small collaborative effort where I was responsible for data processing and analysis, while my partner handled the full-stack development of an application. The app made requests to a Python function to calculate Pokémon damage.

The full project is available at: https://github.com/borjaarcos/Pokeproject 

Here, the work is simplified and presented as Jupyter Notebooks focused on the data and simulation side, showing the core logic I developed.

The notebooks simulate damage output of Pokémon moves against other Pokémon using a simplified damage formula, considering stats, move characteristics, STAB, and type effectiveness. This allows understanding move effectiveness in a clear and generic way across many Pokémon.

## Project Structure
### 01_preprocessing.py
Modifies the structure of the original database (pokemon_data.csv) by splitting composite columns into individual columns to facilitate analysis. **The result is a clean new file called pokemon_data_mod.csv**.

Original data base obtained from: **https://www.kaggle.com/datasets/tanishksharma9905/pokemon-data-csv/data**

Author: **Tanishk Sharma**

### 02_move_API_data_collection.py
Extracts a unique list of moves from the modified database and queries the official Pokémon API to obtain additional information (power, accuracy, type, damage class, etc.) for each move. **This information is saved in the file movimientos_pokemon_info.csv.**

### 03_damage_simulator.py
Uses the processed data from pokemon_data_mod.csv and movimientos_pokemon_info.csv to calculate a simplified estimate of the damage a selected Pokémon can deal with its moves, applying a formula based on stats and type and STAB multipliers.
