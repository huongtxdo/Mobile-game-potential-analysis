# Analyzing mobile games' hit potential using the DNA method

[Aleksandr Enin presented a method](https://www.gamesindustry.biz/how-do-you-evaluate-a-mobile-games-profit-potential) of evaluating a mobile game's profit potential based on its day-1 retention rate among players playing a certain minute of gameplay within the first 10 minutes. That retention graph is called the project's DNA.

## Project structure

```
├── data/                
│   └── cleaned/
│       └── cleaned_date.parquet            # cleaned data
│   └── data.parquet                        # mocked data
├── notebooks/            
│   ├── 01_game_potential.ipynb             # analyzing game's profit potential based on its DNA
│   └── 02_dna_method_improvement.ipynb     # DNA method's counter arguments and suggestions for improvement
├── requirements.txt                        # dependencies required to run the notebooks
└── README.md            
```

## How to run

1. Create and activate a virtual environment
   - On Windows:
   ```
   python -m venv venv
   venv\Scripts\activate
   ```
2. Install project dependencies and make sure all dependecies are installed
    ```
    pip install -r requirements.txt
    ```
3. Register the environment as a Jupyter kernel and select it when prompted
    ```
    python -m ipykernel install --user --name=game_potential_venv
    ```
4. Run the notebooks
5. Deactivate when done
    ```
    deactivate
    ```

## Notes

- The data is made up for the purpose of implementation the DNA methodology. It does not reflect reality.
