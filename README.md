# AppetIte: Smart AI Recipe Generator

AppetIte generates personalized recipes based on the ingredients you have. Using a fine-tuned BART model, it creates recipe names and instructions tailored to your pantry. Whether you want a quick meal or something indulgent, AppetIte has you covered!

## Features
- Generate recipes from text ingredient lists
- Categorize recipes into Healthy, Quick Meals, Indulgent, and Family-Friendly
- Detect common allergens and give safety warnings
- Fast training optimized for local MacBook Air
- Clear recipe names shown with instructions

## Getting Started

### Requirements
- Python 3.8+
- PyTorch (with Apple MPS support if on Mac)
- Transformers, Pandas, Scikit-learn, Tqdm, Rouge-Score
  
### Installation

pip install transformers torch pandas scikit-learn tqdm rouge-score


### Dataset
Put your `AppetIteDataset.csv` in the project folder or update the path in the notebook.

## How to Run
- Open and run the `AppetIte_Optimized_With_Recipe_Names.ipynb` notebook
- Update dataset path if needed
- Run all cells from data loading to fine-tuning and testing
- Use `generate_recipe_with_safety()` function to get recipes programmatically

## Example
result = generate_recipe_with_safety("chicken, rice, vegetables", category="Healthy")
print("Recipe Name:", result['recipe_name'])
print("Instructions:", result['instructions'])
if result['allergens']:
print("Allergen Warning:", result['allergens'])


