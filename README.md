# League of Legends Match Prediction

This project predicts the outcome of League of Legends matches by analyzing various factors such as team composition, player history, champion proficiency, and more. The model uses neural networks and machine learning techniques to predict the probability of a win or loss for a given match.

## Features

- **Match Prediction**: Predicts match outcomes based on team composition, player data, and synergy.
- **Player History**: Automatically fetches player history from the Riot API, analyzing past performance, win rates, most-played champions, and KDA.
- **Champion Analysis**: Classifies champions by playstyle, determines roles, and evaluates synergies within the team.
- **Team Composition**: Evaluates team composition for synergies, counter-picks, and meta effectiveness.
- **Opponent Analysis**: Analyzes the opponent's team composition, counter-picks, and compares strengths and weaknesses.
- **Match Timing**: Considers early-game and late-game strengths to predict match outcomes based on timing.
- **Meta Awareness**: Adjusts predictions based on the current meta, including the most effective strategies and champion picks.
- **Counter-Picks & Synergies**: Identifies counter-champions and synergies to refine predictions.

## Requirements

This project requires a virtual environment with the following dependencies:

- Python 3.x
- `streamlit` - For the web interface
- `torch` - For the prediction model
- `numpy` & `pandas` - For data manipulation
- `matplotlib` - For visualizations
- `requests` - For fetching data from the Riot API

## Installation

### 1. Set Up the Virtual Environment
Create and activate the virtual environment:
```bash
python -m venv new_env
.\new_env\Scripts\activate  # On Windows
source new_env/bin/activate  # On Mac/Linux
```

### 2. Install Dependencies
Install required packages:
```bash
pip install streamlit torch numpy pandas matplotlib requests
```

### 3. Run the Web Interface
Launch the app:
```bash
streamlit run app.py
```

## Usage

1. **Input Team Data**: Enter the team compositions, including the champions each player will be playing.
2. **Automatic Player History**: The app fetches player stats (e.g., win rates, most-played champions) from the Riot API.
3. **View Prediction**: The app generates a win/loss prediction based on the input team compositions, champion analysis, and synergy.

## Future Enhancements

- **Champion Refinement**: Classify champions with more specific roles and combinations.
- **Post-Game Analysis**: Offer suggestions for team composition improvements.
- **More Data Sources**: Integrate third-party stats to enhance analysis.

## License

This project is open-source and available under the MIT License. See the [LICENSE](LICENSE) file for more information.